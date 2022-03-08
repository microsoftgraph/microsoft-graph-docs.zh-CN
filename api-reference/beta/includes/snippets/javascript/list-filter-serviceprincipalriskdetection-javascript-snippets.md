---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: b407f70f7f968edf871d516182077b0590f05730
ms.sourcegitcommit: 77d2ab5018371f153d47cc1cd25f9dcbaca28a95
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/08/2022
ms.locfileid: "63334812"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let servicePrincipalRiskDetections = await client.api('/identityProtection/servicePrincipalRiskDetections')
    .version('beta')
    .filter('riskEventType eq \'investigationsThreatIntelligence\' or riskLevel eq \'medium\'')
    .get();

```