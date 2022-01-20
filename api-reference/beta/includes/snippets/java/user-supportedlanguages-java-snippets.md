---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 2546e33c5bf768af98067649bb4c5685370b82398863df720d64bd212c8366f4
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57273978"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

OutlookUserSupportedLanguagesCollectionPage supportedLanguages = graphClient.me().outlook()
    .supportedLanguages()
    .buildRequest()
    .get();

```