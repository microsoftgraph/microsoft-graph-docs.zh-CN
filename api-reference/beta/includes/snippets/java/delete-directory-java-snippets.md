---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 9fb06b7b51f819c96c9dcf1c9e953569b0e88a7a43d80338a3f407d6d217df0f
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57220938"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.directory().deletedItems("46cc6179-19d0-473e-97ad-6ff84347bbbb")
    .buildRequest()
    .delete();

```