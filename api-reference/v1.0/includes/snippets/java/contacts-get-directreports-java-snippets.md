---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 2b96c745165f4a14eccc1944e237c6843464da84
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50974645"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

DirectoryObjectCollectionWithReferencesPage directReports = graphClient.contacts("{id}").directReports()
    .buildRequest()
    .get();

```