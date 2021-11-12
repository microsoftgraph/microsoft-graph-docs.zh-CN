---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 2dc6b269d01dcf52e2a79f79f97722b870c6c9a2f63a08f514cff1663b9c5e06
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57161399"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

DirectoryObjectCollectionWithReferencesPage directReports = graphClient.contacts("{id}").directReports()
    .buildRequest()
    .get();

```