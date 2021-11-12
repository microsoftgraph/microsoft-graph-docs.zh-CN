---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 5eebced32327ee4fb6857f4cdd47b6e97a2842ce769404b16fff135634be80f3
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57105341"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

GroupCollectionWithReferencesPage allowedGroups = graphClient.print().shares("{printerShareId}").allowedGroups()
    .buildRequest()
    .get();

```