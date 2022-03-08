---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 62ee1f41100766dd1e1ea12c3d825888ba9e1059
ms.sourcegitcommit: 6968f5aaf40089684efb0c38a95f6cca353c1d92
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/16/2022
ms.locfileid: "62854277"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const accessPackageResourceRequest = {
  catalogId: '26ac0c0a-08bc-4a7b-a313-839f58044ba5',
  requestType: 'AdminAdd',
  justification: '',
  accessPackageResource: {
      displayName: 'Faculty cafeteria ordering',
      description: 'Example application',
      url: 'https://myapps.microsoft.com/example.com/signin/Faculty%20cafeteria%20ordering/f1e3b407-942d-4934-9a3f-cef1975cb988/',
      resourceType: 'Application',
      originId: '2f1099a6-d4fc-4cc9-a0ef-ddd3f1bf0b7e',
      originSystem: 'AadApplication',
      attributes: [
        {
          attributeName: 'extension_2b676109c7c74ae2b41549205f1947ed_personalTitle',
          isEditable: true,
          isPersistedOnAssignmentRemoval: true,
          attributeSource: {
              '@odata.type': '#microsoft.graph.accessPackageResourceAttributeQuestion',
              question: {
                  '@odata.type': '#microsoft.graph.accessPackageTextInputQuestion',
                  isRequired: false,
                  sequence: 0,
                  isSingleLineQuestion: true,
                  text: {
                      defaultText: 'Title',
                      localizedTexts: []
                  }
              }
          },
          attributeDestination: {
              '@odata.type': '#microsoft.graph.accessPackageUserDirectoryAttributeStore'
          }
        }
      ]
  }
};

await client.api('/identityGovernance/entitlementManagement/accessPackageResourceRequests')
    .version('beta')
    .post(accessPackageResourceRequest);

```