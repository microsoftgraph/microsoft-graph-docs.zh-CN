---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: b5115c84d5dc8f7b89f7985ec04ef76bea575635
ms.sourcegitcommit: dfa87904fb26dd5161f604f2716ce1d90dad31ed
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/09/2022
ms.locfileid: "63411843"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

ExtensionPropertyCollectionPage extensionProperties = graphClient.applications("fd918e4b-c821-4efb-b50a-5eddd23afc6f").extensionProperties()
    .buildRequest()
    .get();

```