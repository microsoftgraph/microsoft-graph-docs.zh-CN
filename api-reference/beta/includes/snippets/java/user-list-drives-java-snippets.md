---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 588e45ab41ea7c6072e79683c4f929e5f0c8509f2ad5d546581a3416ffe5dec8
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57105180"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

DriveCollectionPage drives = graphClient.users("{userId}").drives()
    .buildRequest()
    .get();

```