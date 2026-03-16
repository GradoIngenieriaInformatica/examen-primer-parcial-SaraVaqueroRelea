db.libros.aggregate([
    {
        $group: {
            _id : "$categoria",
            totalCategorias: {$sum :1}
        }
    }
])