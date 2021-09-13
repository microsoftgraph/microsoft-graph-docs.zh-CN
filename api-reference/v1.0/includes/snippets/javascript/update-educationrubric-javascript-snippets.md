---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: deec94adbca41b4c5f5eeeeaa8e7b7528a6682757ac751516282bdc4a90ff481
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57104987"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const educationRubric = {
  displayName: 'Example Credit Rubric after display name patch'
};

await client.api('/education/me/rubrics/ceb3863e-6912-4ea9-ac41-3c2bb7b6672d')
    .update(educationRubric);

```