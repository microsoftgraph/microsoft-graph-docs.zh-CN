---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 903faf5fbea3713d34fd03a43453c05b96cead364a2e120e56c86bef681119bb
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "56903349"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

DriveItemCollectionPage children = graphClient.me().drive().root().children()
    .buildRequest()
    .get();

```