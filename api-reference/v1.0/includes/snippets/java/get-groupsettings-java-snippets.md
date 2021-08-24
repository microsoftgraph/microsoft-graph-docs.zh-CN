---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: f6eb9f03a32d6b0d7722b4340966670d5bdd2c067e216999a8c329bdad7d28fe
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57333943"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

GroupSettingCollectionPage groupSettings = graphClient.groupSettings()
    .buildRequest()
    .get();

```