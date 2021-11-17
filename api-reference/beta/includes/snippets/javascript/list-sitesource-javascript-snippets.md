---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: b6b85910b2eb93e9079f0f8bf0e6d9a7718048803bb512894afe913f651c8b51
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57162920"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let siteSources = await client.api('/compliance/ediscovery/cases/c816dd6f-5af8-40c5-a760-331361e05c60/legalHolds/277107ff-fee3-41a0-a665-a9d7f6c4824f/siteSources')
    .version('beta')
    .get();

```