# rect-native-select

react-native-select is a highly customizable dropdownlist for android and ios.

# Insallation

`npm install @redmin_delishaj/react-native-select`

Basic Usage

```
import Select, { SelectItem } from '@redmin_delishaj/react-native-select';

const data: SelectItem[] = [
  { text: 'Option 1', value: 1 },
  { text: 'Option 2', value: 2 },
  { text: 'Option 3', value: 3 },
];

const App = () => {

  const [selectedItem, setSelectedItem] = useState<any>();

  return (
      <Select
        data={data}
        onSelect={value => setSelectedItem(value)}
        value={selectedItem}
      />
  );
};
```

Basic Config

```
import Select, { SelectConfig, SelectItem } from '@redmin_delishaj/react-native-select';

const data: SelectItem[] = [
  { text: 'Option 1', value: 1 },
  { text: 'Option 2', value: 2 },
  { text: 'Option 3', value: 3 },
]

const App = () => {

  const [selectedItem, setSelectedItem] = useState<any>();

  const config: SelectConfig = {
    fontSize: 18,
    backgroundColor: '#404040',
    textColor: 'white',
    selectedBackgroundColor: 'white',
    selectedTextColor: 'black',
    selectedFontWeight: 'bold',
  }

  return (
    <Select
      data={data}
      onSelect={value => setSelectedItem(value)}
      value={selectedItem}
      config={config}
    />
  );
};
```
