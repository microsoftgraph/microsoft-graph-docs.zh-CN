---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: e1c5191c42c9d42d08b434cb754b7b9b61ab8365
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50793624"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const informationProtectionAction = {
  contentInfo: {
    '@odata.type': '#microsoft.graph.contentInfo',
    'format@odata.type': '#microsoft.graph.contentFormat',
    format: 'default',
    identifier: null,
    'state@odata.type': '#microsoft.graph.contentState',
    state: 'rest',
    'metadata@odata.type': '#Collection(microsoft.graph.keyValuePair)',
    metadata: [
      {
        '@odata.type': '#microsoft.graph.keyValuePair',
        name: 'MSIP_Label_722a5300-ac39-4c9a-88e3-f54c46676417_Enabled',
        value: 'True'
      },
      {
        '@odata.type': '#microsoft.graph.keyValuePair',
        name: 'MSIP_Label_722a5300-ac39-4c9a-88e3-f54c46676417_Method',
        value: 'Standard'
      },
      {
        '@odata.type': '#microsoft.graph.keyValuePair',
        name: 'MSIP_Label_722a5300-ac39-4c9a-88e3-f54c46676417_SetDate',
        value: '1/1/0001 12:00:00 AM'
      },
      {
        '@odata.type': '#microsoft.graph.keyValuePair',
        name: 'MSIP_Label_722a5300-ac39-4c9a-88e3-f54c46676417_SiteId',
        value: 'cfa4cf1d-a337-4481-aa99-19d8f3d63f7c'
      },
      {
        '@odata.type': '#microsoft.graph.keyValuePair',
        name: 'MSIP_Label_722a5300-ac39-4c9a-88e3-f54c46676417_Name',
        value: 'General'
      },
      {
        '@odata.type': '#microsoft.graph.keyValuePair',
        name: 'MSIP_Label_722a5300-ac39-4c9a-88e3-f54c46676417_ContentBits',
        value: '0'
      },
      {
        '@odata.type': '#microsoft.graph.keyValuePair',
        name: 'MSIP_Label_722a5300-ac39-4c9a-88e3-f54c46676417_ActionId',
        value: '00000000-0000-0000-0000-000000000000'
      }
    ]
  },
  downgradeJustification: {
        justificationMessage: 'The information has been declassified.',
        isDowngradeJustified: true
    }
};

await client.api('/informationProtection/policy/labels/evaluateRemoval')
    .version('beta')
    .post(informationProtectionAction);

```