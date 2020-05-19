---
title: educationOneRosterApiDataProvider 资源
description: 用于在将 OneRoster API 用作输入源时设置学校数据同步配置文件。
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: ca3341c84b79ff25e55be1abf5a8a5a031e84b02
ms.sourcegitcommit: 87966dcd42a0111c5c9987fcae0a491c92022938
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/19/2020
ms.locfileid: "44290383"
---
# <a name="educationonerosterapidataprovider-resource"></a><span data-ttu-id="8703c-103">educationOneRosterApiDataProvider 资源</span><span class="sxs-lookup"><span data-stu-id="8703c-103">educationOneRosterApiDataProvider resource</span></span>

<span data-ttu-id="8703c-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8703c-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8703c-105">用于在将[ONEROSTER API](https://www.imsglobal.org/activity/onerosterlis)用作输入源时设置学校数据同步配置文件。</span><span class="sxs-lookup"><span data-stu-id="8703c-105">Used to set up the school data synchronization profile when the [OneRoster API](https://www.imsglobal.org/activity/onerosterlis) is used as the input source.</span></span>

<span data-ttu-id="8703c-106">派生自[educationSynchronizationDataProvider](educationsynchronizationdataprovider.md)。</span><span class="sxs-lookup"><span data-stu-id="8703c-106">Derived from [educationSynchronizationDataProvider](educationsynchronizationdataprovider.md).</span></span>

## <a name="properties"></a><span data-ttu-id="8703c-107">属性</span><span class="sxs-lookup"><span data-stu-id="8703c-107">Properties</span></span>

| <span data-ttu-id="8703c-108">属性</span><span class="sxs-lookup"><span data-stu-id="8703c-108">Property</span></span> | <span data-ttu-id="8703c-109">类型</span><span class="sxs-lookup"><span data-stu-id="8703c-109">Type</span></span> | <span data-ttu-id="8703c-110">说明</span><span class="sxs-lookup"><span data-stu-id="8703c-110">Description</span></span> |
|:-|:-|:-|
| <span data-ttu-id="8703c-111">**connectionUrl**</span><span class="sxs-lookup"><span data-stu-id="8703c-111">**connectionUrl**</span></span> | <span data-ttu-id="8703c-112">String</span><span class="sxs-lookup"><span data-stu-id="8703c-112">String</span></span> | <span data-ttu-id="8703c-113">指向 OneRoster 实例的连接 URL。</span><span class="sxs-lookup"><span data-stu-id="8703c-113">The connection URL to the OneRoster instance.</span></span> |
| <span data-ttu-id="8703c-114">**schoolsIds**</span><span class="sxs-lookup"><span data-stu-id="8703c-114">**schoolsIds**</span></span> | <span data-ttu-id="8703c-115">String collection</span><span class="sxs-lookup"><span data-stu-id="8703c-115">String collection</span></span> |  <span data-ttu-id="8703c-116">要同步的学校 sourcedIds 的列表。</span><span class="sxs-lookup"><span data-stu-id="8703c-116">The list of school sourcedIds to sync.</span></span> |
| <span data-ttu-id="8703c-117">**providerName**</span><span class="sxs-lookup"><span data-stu-id="8703c-117">**providerName**</span></span> | <span data-ttu-id="8703c-118">String</span><span class="sxs-lookup"><span data-stu-id="8703c-118">String</span></span> | <span data-ttu-id="8703c-119">由[OneRoster 规范](https://www.imsglobal.org/oneroster-v11-final-best-practice-and-implementation-guide#AppA)定义的 OneRoster 服务提供程序名称。</span><span class="sxs-lookup"><span data-stu-id="8703c-119">The OneRoster Service Provider name as defined by the [OneRoster specification](https://www.imsglobal.org/oneroster-v11-final-best-practice-and-implementation-guide#AppA).</span></span> |
| <span data-ttu-id="8703c-120">**connectionSettings**</span><span class="sxs-lookup"><span data-stu-id="8703c-120">**connectionSettings**</span></span> | [<span data-ttu-id="8703c-121">educationSynchronizationConnectionSettings</span><span class="sxs-lookup"><span data-stu-id="8703c-121">microsoft.graph.educationSynchronizationConnectionSettings</span></span>](educationsynchronizationconnectionsettings.md) | <span data-ttu-id="8703c-122">OneRoster 实例的连接设置。</span><span class="sxs-lookup"><span data-stu-id="8703c-122">Connection settings for the OneRoster instance.</span></span> <span data-ttu-id="8703c-123">应为[educationSynchronizationOAuth1ConnectionSettings](educationsynchronizationoauth1connectionsettings.md)或[educationSynchronizationOAuth2ClientCredentialsConnectionSettings](educationsynchronizationoauth2clientcredentialsconnectionsettings.md)的类型类型。</span><span class="sxs-lookup"><span data-stu-id="8703c-123">Should be of type [microsoft.graph.educationSynchronizationOAuth1ConnectionSettings](educationsynchronizationoauth1connectionsettings.md) or [microsoft.graph.educationSynchronizationOAuth2ClientCredentialsConnectionSettings](educationsynchronizationoauth2clientcredentialsconnectionsettings.md).</span></span> |
| <span data-ttu-id="8703c-124">**操作**</span><span class="sxs-lookup"><span data-stu-id="8703c-124">**customizations**</span></span> | [<span data-ttu-id="8703c-125">educationSynchronizationCustomizations</span><span class="sxs-lookup"><span data-stu-id="8703c-125">microsoft.graph.educationSynchronizationCustomizations</span></span>](educationsynchronizationcustomizations.md) | <span data-ttu-id="8703c-126">要应用于同步配置文件的可选自定义项。</span><span class="sxs-lookup"><span data-stu-id="8703c-126">Optional customization to be applied to the synchronization profile.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="8703c-127">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="8703c-127">JSON representation</span></span>
<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.educationoneRosterApiDataProvider"
}-->

```json
{
    "@odata.type": "microsoft.graph.educationoneRosterApiDataProvider",
    "connectionUrl": "String",
    "providerName": "String",
    "schoolsIds": [
        "String"
    ],
    "connectionSettings": {
        "@odata.type": "microsoft.graph.educationSynchronizationOAuth1ConnectionSettings",
        "clientId": "String",
        "clientSecret": "String",
    },
    "customizations": { "@odata.type": "microsoft.graph.educationSynchronizationCustomizations" }
}
```
<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2020-05-06 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "educationOneRosterApiDataProvider resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
      "Error: microsoft.graph.educationoneRosterApiDataProvider/connectionSettings:\r\n      Referenced type microsoft.graph.educationSynchronizationConnectionSettings is not defined in the doc set! Potential suggestion: microsoft.graph.settings"
  ]
}-->