Nama  : Manurung Alex Roger

Kelas : TI.20.A.2

NIM   : 312010478

.

from flask import Flask, jsonify


app = Flask(__name__)


students = [

    {
        "No": "1",
        "nama": "RYANALDI RIVANSYAH",
        "nim": "311610318"
    },
    {
        "No": "2",
        "nama": "RIZKY FEBRIYANTO",
        "nim": "311910250"
    },
    {
        "No": "3",
        "nama": "ERY SHANDY",
        "nim": "312010201"
    },
    {
        "No": "4",
        "nama": "MOHAMMAD SOFIYAN",
        "nim": "312010225"
    },
    {
        "No": "5",
        "nama": "RA'IF EKA RIANDA",
        "nim": "312010254"
    },
    {
        "No": "6",
        "nama": "MUHAMMAD RIFQI RIZQULLAH",
        "nim": "312010263"
    },
    {
        "No": "7",
        "nama": "REZA TARIKI TASER",
        "nim": "312010265"
    },
    {
        "No": "8",
        "nama": "RANGGA SAPUTRA",
        "nim": "312010266"
    },
    {
        "No": "9",
        "nama": "ALINGGA REANDITO",
        "nim": "312010276"
    },
    {
        "No": "10",
        "nama": "EVAROSTIANA DEWI",
        "nim": "312010295"
    },
    {
        "No": "11",
        "nama": "NIA DWI RAHAYU",
        "nim": "312010298"
    },
    {
        "No": "12",
        "nama": "M. HANNATA ZAHRI",
        "nim": "312010318"
    },
    {
        "No": "13",
        "nama": "VERONIKA RUSTIANI DAME SIHOMBING",
        "nim": "312010325"
    },
    {
        "No": "14",
        "nama": "VERONIKA DESNA ERNAYANTI FAU",
        "nim": "312010333"
    },
    {
        "No": "15",
        "nama": "AHMAD ALFIAN CHANDRA",
        "nim": "312010336"
    },
    {
        "No": "16",
        "nama": "MUHAMMAD SAFRI SATRIA PERMANA",
        "nim": "312010337"
    },
    {
        "No": "17",
        "nama": "REKA HANI LATIFAH NURHASANAH",
        "nim": "312010343"
    },
    {
        "No": "18",
        "nama": "SYAHRU RAGA RAMDHANI",
        "nim": "312010354"
    },
    {
        "No": "19",
        "nama": "RAFI HANIF RABBANI",
        "nim": "312010358"
    },
    {
        "No": "20",
        "nama": "ANING KINANTI",
        "nim": "312010364"
    },
    {
        "No": "21",
        "nama": "ARI NUGROHOJATI",
        "nim": "312010366"
    },
    {
        "No": "22",
        "nama": "MOCH.AQILLA FASHA",
        "nim": "312010367"
    },
    {
        "No": "23",
        "nama": "FARIS ARYANO PIRSADA",
        "nim": "312010371"
    },
    {
        "No": "24",
        "nama": "MUHAMMAD RIZKY ABDILLAH",
        "nim": "312010386"
    },
    {
        "No": "25",
        "nama": "HERLIYANSYAH",
        "nim": "312010387"
    },
    {
        "No": "26",
        "nama": "MUHAMMAD IKWANUR DIMAS FAUZI",
        "nim": "312010388"
    },
    {
        "No": "27",
        "nama": "HUMAM FATHURRAHMAN",
        "nim": "312010389"
    },
    {
        "No": "28",
        "nama": "RAYHAN ILHAM RAMANDA",
        "nim": "312010390"
    },
    {
        "No": "29",
        "nama": "MUHAMMAD ARILDA APRILIANTO",
        "nim": "312010399"
    },
    {
        "No": "30",
        "nama": "MUHAMAD FARHAN",
        "nim": "312010400"
    },
    {
        "No": "31",
        "nama": "DEVI SILMA YUNIAR",
        "nim": "312010458"
    },
    {
        "No": "32",
        "nama": "DZAMAR NAWWAF FATIH FIRDAUS",
        "nim": "312010477"
    },
    {
        "No": "33",
        "nama": "MANURUNG ALEX ROGER",
        "nim": "312010478"
    },
    {
        "No": "34",
        "nama": "BA'DO FEBRIANSYAH",
        "nim": "312010485"
    },
    {
        "No": "35",
        "nama": "HELMI SALASFAZRI",
        "nim": "312010486"
    },
    {
        "No": "36",
        "nama": "RAMON MISTER HADI",
        "nim": "312010508"
    },
    {
        "No": "37",
        "nama": "MUHAMMAD NAJAMUDDIN DWI MIHARJA, S.KOM, M.KOM",
        "nim": "Dosen Utama"
    },
]

@app.route('/students', methods=['GET'])
def get_students():
    return jsonify({'students': students})

if __name__ == '__main__':
    app.run(debug=True)
