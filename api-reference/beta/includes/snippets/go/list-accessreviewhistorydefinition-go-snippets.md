---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 7b2a008a66cfce2f129ce7c68d118e5f2ac035f1
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "60992059"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

result, err := graphClient.IdentityGovernance().AccessReviews().HistoryDefinitions().Get(options)


```