# button


import React from 'react'

type PropsType = {
    name: string
    callBack: () => void
    className: string
}
export const Buttons = (props: PropsType) => {
    const onClickHandler = () => {
        props.callBack()
    }

    return (
        <button className={props.className} onClick={onClickHandler}>{props.name}</button>
    );
};
