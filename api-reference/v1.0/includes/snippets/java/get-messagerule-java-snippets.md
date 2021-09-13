---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: a72e171b6a8fad852e51c0810a355d0ca5e496b933fc80b79c82f08454db9a38
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57162966"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

MessageRule messageRule = graphClient.me().mailFolders("inbox").messageRules("AQAAAJ5dZqA=")
    .buildRequest()
    .get();

```