---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 5728947a8e20dd587339f14f086ac8c2f4ec23f30b7da2dd585661929fd99863
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57333350"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.print().shares("{printerShareId}").allowedGroups("{groupId}").reference()
    .buildRequest()
    .delete();

```