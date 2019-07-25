---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 1ce72091d0feacdaceb68cf4f4daba1e88581f0d
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/25/2019
ms.locfileid: "35877232"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.me().onenote().pages("{id}")
    .buildRequest()
    .delete();

```