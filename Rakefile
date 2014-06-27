task :default => 'cophy.pdf'

file 'cophy.pdf' => 'cophy.tex' do |t|
  sh "pdflatex #{t.source}"
end
