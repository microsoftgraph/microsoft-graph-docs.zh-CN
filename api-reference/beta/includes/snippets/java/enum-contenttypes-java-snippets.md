---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 0e35f43f42c2ffc041500b672d9574dd502f2ff05478eab3dc8b2bfe83bd6c32
ms.sourcegitcommit: 24d0ea8e2bcb54c2f397133460c3d26fb0ba705f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/11/2021
ms.locfileid: "60730016"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

ContentTypeCollectionPage contentTypes = graphClient.sites("{site-id}").lists("{list-id}").contentTypes()
    .buildRequest()
    .get();

```