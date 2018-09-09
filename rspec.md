# Quick and Nasty RSpec

Take the Lynda course: Ruby:Testing with RSpec

### Initial Setup

- `$ bundle init`
- add `gem "rspec"` to Gemfile
- `$ bundle install`
- `$ rspec --init`
- `$ mkdir lib`
- ruby code goes in the lib folder (lib/example.rb)
- tests (specs) go in the spec folder (spec/example_spec.rb)

- run with `bundle exec rspec`

### Example RSpec Code

```Ruby
require "example"

describe 'ClassName' do
  it 'does something cool' do
    expect(ClassName.method).to eq('something cool')
  end
end
```

### RSpec Hierarchy

```Ruby
- spec file             example_spec.rb
  - example group       describe
    - nested group      describe / context
      - example         it
        - expectations  expect().to()
```

You can just write out `it "string"` and it will be pending
you can also use `xit` or `xdescribe` at the beginning to skip

[RSpec Cheatsheet](http://www.anchor.com.au/wp-content/uploads/rspec_cheatsheet_attributed.pdf)
