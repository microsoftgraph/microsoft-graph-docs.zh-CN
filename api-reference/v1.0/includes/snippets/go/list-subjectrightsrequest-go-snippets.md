---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 9b43ec8ae23c77201ac466d806ac20620cc73467
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61103262"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

result, err := graphClient.Privacy().SubjectRightsRequests().Get(options)


```