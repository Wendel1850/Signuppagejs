# Signuppagejs
// Função para verificar se os campos estão preenchidos corretamente
function verificarCampos() {
  const nome = document.getElementById('nome').value;
  const email = document.getElementById('email').value;
  const senha = document.getElementById('senha').value;
  const confirmarSenha = document.getElementById('confirmar-senha').value;

  if (nome === '' || email === '' || senha === '' || confirmarSenha === '') {
    document.getElementById('erro').innerHTML = 'Preencha todos os campos';
    return false;
  }

  if (senha !== confirmarSenha) {
