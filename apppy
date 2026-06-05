import streamlit as st

st.set_page_config(page_title="Interacciones de Medicamentos")

st.title("💊 Interacciones de Medicamentos con IA")

medicamento = st.text_input("Ingrese el nombre del medicamento")

if medicamento:

    st.subheader("Interacciones relevantes")

    interacciones = f"""
    Medicamento: {medicamento}

    Interacciones importantes:
    - Alcohol: puede aumentar efectos adversos.
    - Anticoagulantes: pueden modificar la eficacia del tratamiento.
    - Otros medicamentos deben ser revisados por un profesional de salud.
    """

    st.write(interacciones)

    folleto = f"""
    FOLLETO PARA PACIENTES

    Medicamento: {medicamento}

    ¿Para qué sirve?
    Consulte a su médico o farmacéutico.

    Recomendaciones:
    - Tome el medicamento según indicación médica.
    - No exceda la dosis recomendada.
    - Informe cualquier reacción adversa.

    Interacciones importantes:
    - Alcohol
    - Anticoagulantes
    - Otros medicamentos de uso continuo

    En caso de duda consulte a un profesional de la salud.
    """

    st.download_button(
        label="📄 Descargar folleto",
        data=folleto,
        file_name=f"folleto_{medicamento}.txt",
        mime="text/plain"
    )
