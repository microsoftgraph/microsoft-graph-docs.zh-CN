---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: ea25fe1c9edb8d579f7eefdc3869607b8ab788f2d238cdf2b362d66719b66088
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57332364"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Set set = graphClient.termStore().sets("8ed8c9ea-7052-4c1d-a4d7-b9c10bffea6f")
    .buildRequest()
    .get();

```