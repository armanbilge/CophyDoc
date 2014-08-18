task :default => 'cophy.pdf'

require 'rake/clean'
CLEAN.include '*'
CLEAN.exclude 'Rakefile'
CLEAN.exclude 'cophy.tex'
CLEAN.exclude 'cophy.pdf'
CLOBBER.add 'cophy.pdf'

file 'cophy.pdf' => 'cophy.tex' do |t|
  (0..2).each do
    sh "pdflatex #{t.source}"
  end
end
