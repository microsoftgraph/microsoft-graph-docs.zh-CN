---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 9fd74cc0ab9660c0c3c509c3b191acef54aae9ab45356dcd59c7cde89dec5384
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "56902377"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.print().printerShares("{id}").allowedUsers("{id}").reference()
    .buildRequest()
    .delete();

```