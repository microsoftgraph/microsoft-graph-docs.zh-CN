---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 1f7e0b759e5dee4cef5356869df2889c2f39e06c
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50960510"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IDirectoryObjectCollectionWithReferencesPage ownedObjects = graphClient.me().ownedObjects()
    .buildRequest()
    .get();

```