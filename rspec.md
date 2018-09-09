# Quick and Nasty RSpec

## Initial Setup

- `bundle init`
- add gem "rspec" to Gemfile
- `bundle install`
- `rspec --init`
- `mkdir lib`
- ruby code goes in the lib folder (lib/example.rb)
- tests (specs) go in the spec folder (spec/example_spec.rb)

## Example RSpec Code

```Ruby
require "example"

describe 'ClassName' do
  it 'does something cool' do
    expect(ClassName.something).to eq('cool')
  end
end
```

RSpec Hierarchy

```Ruby
- spec file             example_spec.rb
  - example group       describe
    - nested group      describe / context
      - example         it
        - expectations  expect().to()
```

You can just write out `it "string"` and it will be pending
you can also use `xit` at the beginning to skip
