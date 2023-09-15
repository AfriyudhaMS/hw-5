# hw-5
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Pendaftaran Pendaftar</title>
    <!-- Include Bootstrap CSS -->
    <link href="https://cdn.jsdelivr.net/npm/bootstrap@5.3.0/dist/css/bootstrap.min.css" rel="stylesheet">
</head>
<body>
    <div class="container mt-5">
        <h1 class="text-center">Pendaftaran (Registrasi)</h1>
        <ul class="nav nav-tabs" id="myTabs" role="tablist">
            <li class="nav-item" role="presentation">
                <a class="nav-link active" id="registrasi-tab" data-bs-toggle="tab" href="#registrasi" role="tab" aria-controls="registrasi" aria-selected="true">Registrasi</a>
            </li>
            <li class="nav-item" role="presentation">
                <a class="nav-link" id="list-tab" data-bs-toggle="tab" href="#list" role="tab" aria-controls="list" aria-selected="false">List Pendaftar</a>
            </li>
        </ul>
        <div class="tab-content" id="myTabsContent">
            <div class="tab-pane fade show active" id="registrasi" role="tabpanel" aria-labelledby="registrasi-tab">
                <form id="registration-form" onsubmit="return validateForm()">
                    <div class="mb-3">
                        <label for="nama" class="form-label">Nama:</label>
                        <input type="text" class="form-control" id="nama" name="nama" minlength="10" required>
                    </div>
                    <div class="mb-3">
                        <label for="umur" class="form-label">Umur:</label>
                        <input type="number" class="form-control" id="umur" name="umur" min="25" required>
                    </div>
                    <div class="mb-3">
                        <label for="uang-sangu" class="form-label">Uang Sangu (100 ribu - 1 juta):</label>
                        <input type="number" class="form-control" id="uang-sangu" name="uang-sangu" min="100000" max="1000000" required>
                    </div>
                    <button type="submit" class="btn btn-primary">Daftar</button>
                </form>
            </div>
            <div class="tab-pane fade" id="list" role="tabpanel" aria-labelledby="list-tab">
                <table class="table">
                    <thead>
                        <tr>
                            <th>Nama</th>
                            <th>Umur</th>
                            <th>Uang Sangu</th>
                        </tr>
                    </thead>
                    <tbody id="pendaftar-list">
                    </tbody>
                </table>
                <p id="resume"></p>
            </div>
        </div>
    </div>

    <!-- Include Bootstrap JS -->
    <script src="https://cdn.jsdelivr.net/npm/bootstrap@5.3.0/dist/js/bootstrap.min.js"></script>

    <script>
        // JavaScript code (unchanged from previous example)
    </script>
</body>
</html>
