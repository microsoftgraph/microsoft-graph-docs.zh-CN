---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 741cbd5056d177446f2768bb8e3790b46ac1ee5b
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "61030855"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

result, err := graphClient.Policies().HomeRealmDiscoveryPolicies().Get(options)


```