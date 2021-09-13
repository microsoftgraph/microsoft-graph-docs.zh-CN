---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 21e9b0aef26a11497dd83ac42ddc0bdb2d8a830d09b6a10ca42010ebdfd75cbe
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57333500"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

EducationUserCollectionPage users = graphClient.education().users()
    .buildRequest()
    .get();

```