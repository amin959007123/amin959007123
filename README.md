- 👋 Hi, I’m @amin959007123
- 👀 I’m interested in ...
- 🌱 I’m currently learning ...
- 💞️ I’m looking to collaborate on ...
- 📫 How to reach me ...

<!---
amin959007123/amin959007123 is a ✨ special ✨ repository because its `README.md` (this file) appears on your GitHub profile.
You can click the Preview link to take a look at your changes.
--->async function updateGoogleSheets(count) {
  try {
    await gapi.client.sheets.spreadsheets.values.update({
      spreadsheetId: '1nUsjthmeCT5nptfsL9VhlEaa85R7stkqIDPg7RZG3Zk',
      range: 'follow!A1',
      valueInputOption: 'USER_ENTERED',
      values: [[count]],
    });
  } catch (error) {
    console.error('Error updating Google Sheets:', error);
  }
}
