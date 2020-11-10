---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 6f7551a309c63d41051f04f5861f35e902956820
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/10/2020
ms.locfileid: "48981715"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Notebook notebook = new Notebook();
notebook.displayName = "Notebook name";

graphClient.me().onenote().notebooks()
    .buildRequest()
    .post(notebook);

```