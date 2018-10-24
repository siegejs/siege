# Siege
A modular web component library.

## Roadmap
* [ ]Proxy based reactive data binding
* [ ]Web Component lifecycle
* [ ]React component compatibility(JSX)
* [ ]Single file component

## Design

```Hello.siege
<style lang='less' scoped>
  .hello {
    color: pink;
  }
</style>

<script>
import {Component} from 'siege';

export default class Hello extends Component {
  state = {
    label: 'Hello',
  }
  
  contructor(props) {
    super(props);
  }
  
  render() {
    return <div class='hello' onClick={this.handleClick}>{this.state.label}!</div>; 
  }
  
  handleClick = (e) => {
    this.setState({
      label: 'Hello again',
    })
  }
}
  
</script>
```
