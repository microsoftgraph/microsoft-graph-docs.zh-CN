---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 94c58b6493e2d9808eb51058ee4b7801d160cae2
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "61033270"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

result, err := graphClient.DeviceManagement().VirtualEndpoint().SupportedRegions().Get(options)


```