---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 4aeb7a18a73d952e63fe1d37a54c83bbe6cdd956
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50974492"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

DirectoryObjectCollectionWithReferencesPage registeredDevices = graphClient.me().registeredDevices()
    .buildRequest()
    .get();

```