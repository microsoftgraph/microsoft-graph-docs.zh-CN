---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 4fb562230a7cf9320fb661a5f9372db58de6684f
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61097070"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

result, err := graphClient.TenantRelationships().ManagedTenants().AggregatedPolicyCompliances().Get(options)


```