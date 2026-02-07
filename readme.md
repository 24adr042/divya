import streamlit as st

st.title("Personal Health Coach AI")

age = st.number_input("Enter Age", 1, 100)
bp = st.number_input("BP", 80, 200)

if bp > 140:
    st.warning("High BP detected. Reduce salt & walk daily.")
else:
    st.success("BP is normal. Keep it up!")
