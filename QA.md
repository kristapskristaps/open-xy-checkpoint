# Device checks

Record SDK/extension commits, candidate OS SHA-256 and layout. Test a disposable
project containing synth, sample, auxiliary and SDK-machine tracks.

- [ ] Metronome tap, Metronome + M2, Shift + Metronome and browser/naming controls
  retain stock behavior. Check both orders of releasing every chord.
- [ ] Metronome + plus stores once; holding plus does not repeatedly store.
- [ ] Edit notes, locks, components, length/scale, sounds, levels, pan, sends
  and mutes. Recall restores every captured value.
- [ ] Change samples and trims after storing; recall restores them. Exercise
  sample-memory pressure and retained assignments.
- [ ] Exercise different active and sound-link source patterns. Check the
  documented effects on other scenes sharing them.
- [ ] Exercise SDK drums, sample engines and control machines with saved state.
- [ ] Playback/external sync retain position. Listen for stalls, missing samples,
  stuck notes and discontinuities. Record timing on the exact image.
- [ ] Metronome + Record recovers the pre-recall state once, including SDK state.
  A redundant recall preserves this useful recovery state.
- [ ] No checkpoint, wrong scene, recording and changed pattern counts refuse
  without partial edits. Failed stores preserve the old checkpoint.
- [ ] New/load/reload project clears both states, including same-project reload.
- [ ] Stock undo and Retrospective capture still work after recall/recovery.
- [ ] Save/autosave does not move the checkpoint. Restart clears it.
