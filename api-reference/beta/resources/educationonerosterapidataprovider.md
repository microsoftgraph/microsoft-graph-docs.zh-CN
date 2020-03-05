---
title: educationOneRosterApiDataProvider 资源
description: 用于在将 OneRoster API 用作输入源时设置学校数据同步配置文件。
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: 540a508ae3ac7d2b2ecf0f4cec2862b1331e4958
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42501526"
---
# <a name="educationonerosterapidataprovider-resource"></a><span data-ttu-id="7d044-103">educationOneRosterApiDataProvider 资源</span><span class="sxs-lookup"><span data-stu-id="7d044-103">educationOneRosterApiDataProvider resource</span></span>

<span data-ttu-id="7d044-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="7d044-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7d044-105">用于在将[ONEROSTER API](https://www.imsglobal.org/activity/onerosterlis)用作输入源时设置学校数据同步配置文件。</span><span class="sxs-lookup"><span data-stu-id="7d044-105">Used to set up the school data synchronization profile when the [OneRoster API](https://www.imsglobal.org/activity/onerosterlis) is used as the input source.</span></span>

<span data-ttu-id="7d044-106">派生自[educationSynchronizationDataProvider](educationsynchronizationdataprovider.md)。</span><span class="sxs-lookup"><span data-stu-id="7d044-106">Derived from [educationSynchronizationDataProvider](educationsynchronizationdataprovider.md).</span></span>

## <a name="properties"></a><span data-ttu-id="7d044-107">属性</span><span class="sxs-lookup"><span data-stu-id="7d044-107">Properties</span></span>

| <span data-ttu-id="7d044-108">属性</span><span class="sxs-lookup"><span data-stu-id="7d044-108">Property</span></span> | <span data-ttu-id="7d044-109">类型</span><span class="sxs-lookup"><span data-stu-id="7d044-109">Type</span></span> | <span data-ttu-id="7d044-110">说明</span><span class="sxs-lookup"><span data-stu-id="7d044-110">Description</span></span> |
|:-|:-|:-|
| <span data-ttu-id="7d044-111">**connectionUrl**</span><span class="sxs-lookup"><span data-stu-id="7d044-111">**connectionUrl**</span></span> | <span data-ttu-id="7d044-112">String</span><span class="sxs-lookup"><span data-stu-id="7d044-112">String</span></span> | <span data-ttu-id="7d044-113">指向 OneRoster 实例的连接 URL。</span><span class="sxs-lookup"><span data-stu-id="7d044-113">The connection URL to the OneRoster instance.</span></span> |
| <span data-ttu-id="7d044-114">**schoolsIds**</span><span class="sxs-lookup"><span data-stu-id="7d044-114">**schoolsIds**</span></span> | <span data-ttu-id="7d044-115">String 集合</span><span class="sxs-lookup"><span data-stu-id="7d044-115">String collection</span></span> |  <span data-ttu-id="7d044-116">要同步的学校 sourcedIds 的列表。</span><span class="sxs-lookup"><span data-stu-id="7d044-116">The list of school sourcedIds to sync.</span></span> |
| <span data-ttu-id="7d044-117">**providerName**</span><span class="sxs-lookup"><span data-stu-id="7d044-117">**providerName**</span></span> | <span data-ttu-id="7d044-118">String</span><span class="sxs-lookup"><span data-stu-id="7d044-118">String</span></span> | <span data-ttu-id="7d044-119">由[OneRoster 规范](https://www.imsglobal.org/oneroster-v11-final-best-practice-and-implementation-guide#AppA)定义的 OneRoster 服务提供程序名称。</span><span class="sxs-lookup"><span data-stu-id="7d044-119">The OneRoster Service Provider name as defined by the [OneRoster specification](https://www.imsglobal.org/oneroster-v11-final-best-practice-and-implementation-guide#AppA).</span></span> |
| <span data-ttu-id="7d044-120">**connectionSettings**</span><span class="sxs-lookup"><span data-stu-id="7d044-120">**connectionSettings**</span></span> | [<span data-ttu-id="7d044-121">educationSynchronizationConnectionSettings</span><span class="sxs-lookup"><span data-stu-id="7d044-121">microsoft.graph.educationSynchronizationConnectionSettings</span></span>](educationsynchronizationconnectionsettings.md) | <span data-ttu-id="7d044-122">OneRoster 实例的连接设置。</span><span class="sxs-lookup"><span data-stu-id="7d044-122">Connection settings for the OneRoster instance.</span></span> <span data-ttu-id="7d044-123">应为[educationSynchronizationOAuth1ConnectionSettings](educationsynchronizationoauth1connectionsettings.md)或[educationSynchronizationOAuth2ClientCredentialsConnectionSettings](educationsynchronizationoauth2clientcredentialsconnectionsettings.md)的类型类型。</span><span class="sxs-lookup"><span data-stu-id="7d044-123">Should be of type [microsoft.graph.educationSynchronizationOAuth1ConnectionSettings](educationsynchronizationoauth1connectionsettings.md) or [microsoft.graph.educationSynchronizationOAuth2ClientCredentialsConnectionSettings](educationsynchronizationoauth2clientcredentialsconnectionsettings.md).</span></span> |
| <span data-ttu-id="7d044-124">**操作**</span><span class="sxs-lookup"><span data-stu-id="7d044-124">**customizations**</span></span> | [<span data-ttu-id="7d044-125">educationSynchronizationCustomizations</span><span class="sxs-lookup"><span data-stu-id="7d044-125">microsoft.graph.educationSynchronizationCustomizations</span></span>](educationsynchronizationcustomizations.md) | <span data-ttu-id="7d044-126">要应用于同步配置文件的可选自定义项。</span><span class="sxs-lookup"><span data-stu-id="7d044-126">Optional customization to be applied to the synchronization profile.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="7d044-127">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="7d044-127">JSON representation</span></span>
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
