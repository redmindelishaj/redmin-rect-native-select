# redmin-rect-native-select

react-native-select is a highly customizable dropdownlist for android and ios.

# Insallation

`npm install @redmin_delishaj/react-native-select`

Basic Usage:

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
