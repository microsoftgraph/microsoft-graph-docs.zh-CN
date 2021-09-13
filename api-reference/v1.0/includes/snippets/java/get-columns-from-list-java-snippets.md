---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 563b53ef8d6994b156a0698ea5d80f560ef371e4
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "59062986"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

ColumnDefinitionCollectionPage columns = graphClient.sites("{site-id}").lists("{list-id}").columns()
    .buildRequest()
    .get();

```