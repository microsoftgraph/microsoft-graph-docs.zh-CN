---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: a80938fb205cf6c06f9054a2a195ddd204954b55
ms.sourcegitcommit: 9a5facff47a8d4e05ecd2c6cd68294a948c47c4d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2021
ms.locfileid: "49945487"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var openShift = await graphClient.Teams["{id}"].Schedule.OpenShifts["OPNSHFT_577b75d2-a927-48c0-a5d1-dc984894e7b8"]
    .Request()
    .GetAsync();

```