---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 3a36de1141872a81959c696e60a7e5c058f1b2e2
ms.sourcegitcommit: 77d2ab5018371f153d47cc1cd25f9dcbaca28a95
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/08/2022
ms.locfileid: "63338328"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const acronym = {
  displayName: 'DNN',
  standsFor: 'Deep Neural Network',
  description: 'A deep neural network is a neural network with a certain level of complexity, a neural network with more than two layers.',
  webUrl: 'http://microsoft.com/deep-neural-network',
  state: 'draft'
};

await client.api('/search/acronyms')
    .version('beta')
    .post(acronym);

```