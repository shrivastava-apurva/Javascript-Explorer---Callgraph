import React, {Component} from 'react';
//Below is a functional components

// const SearchBar = () => {
//   return <input />//create HTML input where user can type into
//
// };


// Now we are making similar class component -- for communicating state and
//communicate with other components effectively

class SearchBar extends Component{

  constructor(props) {
    super(props);//calling constructor of parent class - Component with super

    this.state = {term: ''};// we can use any property name
  }
  render () {
    // return <input onChange = {this.onInputChange}/>;

    return (
      <div className = "search-bar">
        <input
        value = {this.state.term}//making input as a controlled input here
        onChange =  {event => this.onInputChange(event.target.value)} />

      </div>
    );
  }

  onInputChange(term) {
  this.setState({term});
  this.props.onSearchTermChange(term);
  }
  // onInputChange(event) { //event handler called with event object -- can be e or eve etc
  //   console.log(event.target.value);
  // }
}

//instance
// new SearchBar
export default SearchBar;
