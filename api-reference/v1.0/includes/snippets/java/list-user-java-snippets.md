---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: a54c285d50b3717150a93d654adb1e246ad2bc35
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50968457"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

UserCollectionWithReferencesPage allowedUsers = graphClient.print().shares("{printerShareId}").allowedUsers()
    .buildRequest()
    .get();

```