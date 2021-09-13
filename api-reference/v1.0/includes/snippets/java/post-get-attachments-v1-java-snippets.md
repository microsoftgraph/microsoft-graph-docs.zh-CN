---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 9993d3edf281e6e1842cf9385d461d719985b7f1c6b03cdfb72a87200309772d
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57162559"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

AttachmentCollectionPage attachments = graphClient.groups("1848753d-185d-4c08-a4e4-6ee40521d115").threads("AAQkADJfolA==").posts("AAMkADJ-aHAAA=").attachments()
    .buildRequest()
    .get();

```