# React-Native-Tags

[![Build Status](https://travis-ci.org/peterp/react-native-tags.svg?branch=master)](https://travis-ci.org/peterp/react-native-tags)

A component that allows you to input text and formats the text into a tag when a space or comma is entered.

```
import React from 'react';
import Tags from 'react-native-tags';
const UselessComponent = () => <Tags 
  initialText=""
  initialTags={['dog', 'cat', 'chicken]}
  onChangeTags={() => noop}
  onTagPress={ (index, tagLabel, event) => console.log(index, tagLabel, event) }
  inputStyle={{ backgroundColor: 'white' }}
/>;
```

## Props

**initialText** PropTypes.string

Populates the text input.

**initialTags** PropTypes.array

Populates the tags.

**onTagsChange** PropTypes.func

Callback that is called when a tag is added or removed.

**onTagPress**  PropTypes.func

Callback that is called when a tag is pressed. Receive (index, tagLabel, event) 

**inputStyle**  PropTypes.object

Object to style the TextInput component