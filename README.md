import React from 'react';
import { Link } from 'react-router-dom';

function ProductItem({ product }) {
  return (
    <div>
      <Link to={`/product/${product.id}`}>
        <h2>{product.name}</h2>
        <p>${product.price}</p>
      </Link>
    </div>
  );
}

export default ProductItem;
