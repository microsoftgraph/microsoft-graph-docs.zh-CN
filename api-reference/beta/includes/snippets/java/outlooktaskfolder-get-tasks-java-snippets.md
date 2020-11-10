---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: d1809b73567ed5a255401985d3d3a28d87adb0f6
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/10/2020
ms.locfileid: "48974806"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IOutlookTaskCollectionPage tasks = graphClient.me().outlook().taskFolders("AAMkADIyAAAhrbPWAAA=").tasks()
    .buildRequest()
    .get();

```