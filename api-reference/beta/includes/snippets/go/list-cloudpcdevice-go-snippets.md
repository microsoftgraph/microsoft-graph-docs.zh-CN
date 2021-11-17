---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 1b2481adcbde5b1b56a76b8f2315faf87051ad61
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "61014684"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

result, err := graphClient.TenantRelationships().ManagedTenants().CloudPcDevices().Get(options)


```