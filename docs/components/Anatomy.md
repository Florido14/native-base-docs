# Anatomy

Automatically animates views to their new positions.<br />
A common way to use [NativeBase](http://nativebase.io/) screen structure is to have all the components within <code>&lt;Container></code>.

<table>
  <thead>
    <tr style="border-style: hidden">
      <th style="border-style: hidden">IOS</th>
      <th>Android</th>
    </tr>
  </thead>
  <thead>
    <tr style="border-style: hidden">
      <th style="border-style: hidden"><img height="470" width="270" src="https://raw.githubusercontent.com/GeekyAnts/NativeBase-KitchenSink/0.5.13/Screenshots/iOS/anatomy.png" alt="" /></th>
      <th><img height="470" width="270" src="https://raw.githubusercontent.com/GeekyAnts/NativeBase-KitchenSink/0.5.13/Screenshots/android/anatomy.png" alt="" /></th>
    </tr>
  </thead>
</table>

**Contents:**
* [Header](/docs/components/Header.md)
* [Content](/docs/components/Content.md)


*General Syntax*
<pre><code class="language-jsx">import React, { Component } from 'react';
import { Container, Header, Title, Content, Footer, FooterTab, Button, Icon } from 'native-base';
​
export default class AnatomyExample extends Component {
    render() {
        return (
            &lt;Container>
                &lt;Header>
                    &lt;Title>Header&lt;/Title>
                &lt;/Header>

                &lt;Content>
                    // Your main content goes here
                &lt;/Content>

                &lt;Footer>
                    &lt;FooterTab>
                        &lt;Button transparent>
                            &lt;Icon name='ios-call' />
                        &lt;/Button>  
                    &lt;/FooterTab>
                &lt;/Footer>
            &lt;/Container>
        );
    }
}</code></pre>



* [NativeBase](http://nativebase.io/) provides its own frame component, named after <code>&lt;Container></code>.
* All the components should be included within the Container.
* Container takes mainly three components: <code>&lt;Header></code>, <code>&lt;Content></code> and <code>&lt;Footer></code>.
* Container comes with its predefined stylesheet, with an added advantage of accepting user-defined styles.
* Usage of Container's <code>Header</code> component is very similar to your HTML &lt;head>. So is with <code>Footer</code>.
* The <code>Content</code> component of Container is nothing but the body section of your screen.<br /><br />

    **Configuration**
    <table class="table table-bordered">
        <thead>
            <tr>
                <th>Property</th>
                <th>Default</th>
                <th>Option</th>
                <th width="50%">Description</th>
            </tr>
        </thead>
        <tbody>
            <tr>
                <td>&lt;Header></td>
                <td> - </td>
                <td> - </td>
                <td>Renders as Header (navbar) of your screen.<br />
                    Input values: Button, Title (Text).
                </td>
            </tr>
            <tr>
                <td>&lt;Content></td>
                <td> - </td>
                <td> - </td>
                <td>Represents the main content of your screen.<br />
                    There can be only one <code style="background-color: #FFF">&lt;Content></code> component in a screen.
                </td>
            </tr>
            <tr>
                <td>&lt;Footer></td>
                <td> - </td>
                <td> - </td>
                <td>Renders as Footer of your screen.<br />
                    Input values: FooterTab
                    </a>
                </td>
            </tr>
        </tbody>
    </table>