---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 03367a7baf178893d52a99bb2d3a112dc33564f1
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61076990"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

User user = graphClient.users("{id | userPrincipalName}")
    .buildRequest()
    .select("displayName,givenName,postalCode,identities")
    .get();

```