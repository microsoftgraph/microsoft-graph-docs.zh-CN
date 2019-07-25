---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 9d54db32f4cf46716db1f0ec6ea6b56ce33c8693
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/25/2019
ms.locfileid: "35888075"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Content {size} = graphClient.me().drive().items("{item-id}").thumbnails("{thumb-id}").{size}()
    .buildRequest()
    .get();

```