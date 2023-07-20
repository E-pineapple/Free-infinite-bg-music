# Free-infinite-bg-music
free music for a background of anything you want!!(it goes on forever, on Sonic Pi btw
live_loop :fob do
  sample :drum_bass_soft, rate: 0.2
  sleep 3
end

live_loop :bar do
  use_synth :kalimba
  play_pattern_timed chord(:E3, :m7), 0.5
  sleep 1
  play_pattern_timed chord(:E3, :dim7), 0.5
  sleep 1
end


live_loop :flibble do
  use_synth :kalimba
  sleep 2
  play_pattern_timed chord(:E4, :m), 0.5
  sleep 2.5
end
live_loop :egg do
  use_synth :kalimba
  sleep 3
  play :e5
  sleep 6
  play :e7, release: 4
  sleep 1
end
live_loop :knee do
  use_synth :dull_bell
  sleep 1
  play :c2
  sleep 2
end

live_loop :fee do
  sample :ambi_drone, rate: 0.15
  sleep 1
end
with_fx :echo, phase: 4 do
  live_loop :fii do
    use_synth :kalimba
    sleep 4
    play :b5
    sleep 3
    play :e6, release: 2
    sleep 1
  end
end

live_loop :fo do
  sample :elec_plip, rate: 3
  sleep 1
end

live_loop :fum do
  sample :elec_tick, rate: 5
  sleep 3
end



