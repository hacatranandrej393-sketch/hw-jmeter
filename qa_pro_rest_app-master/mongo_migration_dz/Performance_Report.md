Collection Schemas
1. Users
| Field | Type | Description |
| :--- | :--- | :--- |
| `_id` | String | Unique user ID. |
| `firstName` | String | User first name. |
| `lastName` | String | User last name. |
| `email` | String | Unique email. |
| `password` | String | Hashed password. |

2. UserProfile
| Field | Type | Description |
| :--- | :--- | :--- |
| `_id` | String | Unique profile ID. |
| `userId` | String | Reference to Users. |
| `country` | String | User country. |
| `photoFilename`| String | Avatar filename. |
| `dateOfBirth` | String | Birth date (ISO). |

3. CarBrands
| Field | Type | Description |
| :--- | :--- | :--- |
| `_id` | String | Unique brand ID. |
| `brandName` | String | Brand name (e.g., BMW). |

 4. CarsModels
| Field | Type | Description |
| :--- | :--- | :--- |
| `_id` | String | Unique model ID. |
| `brandId` | String | Reference to CarBrands. |
| `modelName` | String | Model name (e.g., X5). |

 5. Cars
| Field | Type | Description |
| :--- | :--- | :--- |
| `_id` | String | Unique car ID. |
| `userId` | String | Reference to Users (owner). |
| `modelId` | String | Reference to CarsModels. |
| `milage` | Number | Car mileage. |
| `productionYear`| Number | Year of manufacture. |