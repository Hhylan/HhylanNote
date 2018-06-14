import { ImagePicker, WhiteSpace, WingBlank } from 'antd-mobile'
import React from 'react'
import { View } from 'react-native'
import { connect } from 'react-redux'

const data = [
  {
    url: 'https://zos.alipayobjects.com/rmsportal/PZUUCKTRIHWiZSY.jpeg',
    id: '2121'
  },
  {
    url: 'https://zos.alipayobjects.com/rmsportal/hqQWgTXdrlmVVYi.jpeg',
    id: '2122'
  }
]

export default class UploadImagePicker extends React.Component {
  state = {
    files: data,
    multiple: true
  }

  handleFileChange = (files: any) => {
    console.log(files)
    this.setState({
      files,
    });
  }

  render () {
    const { files } = this.state
    return (
      <WingBlank>
        <ImagePicker
          onChange={this.handleFileChange}
          files={this.state.files}
        />

        <WhiteSpace />
      </WingBlank>
    )
  }
}

