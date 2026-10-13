# T-Intervalos recovered behavior

Sources: REA managed metadata of Assembly-CSharp.dll; complete decoded CIL saved cil-readable.txt; Unity serialized objects (GameObject/Transform/MonoBehaviour) in level2 exercise selector; TextAssets resources.assets/sharedassets.

Modes0 Tom e Semitom,1 Classificação Básica,2 Classificação Completa,3 Auditivo. Phase counts6/8/8/8. Exact serialized phase configs in exercise-configs.json and merged gameplay.json. Category difficulty/per-profile progression/feedback/timer rules match T-Escalas. Values differ: see gameplay.json. Compound includes all simple/compound up to14th, distances ±23; simple±12. Unison included in Basic/Complete/Auditory; Tom/Semitom ±1/±2 only.

Basic task ordinal based diatonic distance. Complete two steps ordinal then quality; no hit until quality correct. Incorrect ordinal fails question. Back button changes to ordinal before submitting quality. Qualities0Perfect,1Major,2Minor,3Diminished,4Augmented displayed Justa/Maior/Menor/Dim/Aum. Compound quality judged modulo octave. Hearing task semitone magnitude, options depend on HearingType: tonic-third-fifth-octave=[0,4,7,12]; natural=[0,2,4,5,7,9,11,12]; chromatic=[0..12]; tone/semitone=[1,2].

Generator: AllNotes60 entries G octave0 through F# octave5, sharp spelling. Allowed first/second relative clef offsets2..36 inclusive; offsets treble21,bass0,alto10. Random first note rejection ensures in selected pitch collection; random signed distance rejection ensures type direction, second allowed note range+scale, interval membership after spelling. Harmonic excludes negative; Asc excludes negative; Desc excludes positive; both allows both. Mixed chooses harmonic or both melodic with equal odds per attempt.

Keys complete fifthcycle Cb,Gb,Db,Ab,Eb,Bb,F,C,G,D,A,E,B,F#,C#. Scale Chromatic all semitones; Major and Minor use selected key major collection. Minor fixed tonic relative minor (Ckey -> A); fixed-root applied only diatonic, Chromatic ignores fixation. Correct key spelling converts canonical sharps to matching scale note letters/accidentals.

Practice mode -> subtype if auditory -> interval type -> simple/compound only Basic/Complete -> scale -> key/root -> fixed/random -> clef if visual; auditory launches without clef. Finalizar ends stopwatch and report time/hits/errors. Comparison is theory, not fifth gameplay category. Theory TextAssets include all visible menu chapters and instrumental examples.

Artifacts: managed-members.json (REA-derived member subset), instructions.json complete opcode decoding, cil-readable.txt readable CIL, static-arrays.json exact embedded signed interval arrays, exercise-configs.json30 phase bindings, gameplay.json normalized config, texts30 files, level*-strings and mainData-strings build/labels.
