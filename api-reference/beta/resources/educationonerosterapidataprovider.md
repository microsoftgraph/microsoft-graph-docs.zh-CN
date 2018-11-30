---
title: educationOneRosterApiDataProvider 资源
description: 用于 OneRoster API 用作输入源时设置学校数据同步配置文件。
ms.openlocfilehash: 0fd9c87c9934fc86d4e6788a5db42eb036fdb04f
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27045087"
---
# <a name="educationonerosterapidataprovider-resource"></a><span data-ttu-id="e35cf-103">educationOneRosterApiDataProvider 资源</span><span class="sxs-lookup"><span data-stu-id="e35cf-103">educationOneRosterApiDataProvider resource</span></span>

> <span data-ttu-id="e35cf-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="e35cf-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="e35cf-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="e35cf-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="e35cf-106">用于[OneRoster API](https://www.imsglobal.org/activity/onerosterlis)用作输入源时设置学校数据同步配置文件。</span><span class="sxs-lookup"><span data-stu-id="e35cf-106">Used to set up the school data synchronization profile when the [OneRoster API](https://www.imsglobal.org/activity/onerosterlis) is used as the input source.</span></span>

<span data-ttu-id="e35cf-107">派生自[educationSynchronizationDataProvider](educationsynchronizationdataprovider.md)。</span><span class="sxs-lookup"><span data-stu-id="e35cf-107">Derived from [educationSynchronizationDataProvider](educationsynchronizationdataprovider.md).</span></span>

## <a name="properties"></a><span data-ttu-id="e35cf-108">属性</span><span class="sxs-lookup"><span data-stu-id="e35cf-108">Properties</span></span>

| <span data-ttu-id="e35cf-109">属性</span><span class="sxs-lookup"><span data-stu-id="e35cf-109">Property</span></span> | <span data-ttu-id="e35cf-110">类型</span><span class="sxs-lookup"><span data-stu-id="e35cf-110">Type</span></span> | <span data-ttu-id="e35cf-111">说明</span><span class="sxs-lookup"><span data-stu-id="e35cf-111">Description</span></span> |
|:-|:-|:-|
| <span data-ttu-id="e35cf-112">**connectionUrl**</span><span class="sxs-lookup"><span data-stu-id="e35cf-112">**connectionUrl**</span></span> | <span data-ttu-id="e35cf-113">字符串</span><span class="sxs-lookup"><span data-stu-id="e35cf-113">String</span></span> | <span data-ttu-id="e35cf-114">连接到 OneRoster 实例 URL。</span><span class="sxs-lookup"><span data-stu-id="e35cf-114">The connection URL to the OneRoster instance.</span></span> |
| <span data-ttu-id="e35cf-115">**schoolsIds**</span><span class="sxs-lookup"><span data-stu-id="e35cf-115">**schoolsIds**</span></span> | <span data-ttu-id="e35cf-116">String 集合</span><span class="sxs-lookup"><span data-stu-id="e35cf-116">String collection</span></span> |  <span data-ttu-id="e35cf-117">学校 sourcedIds 同步的列表。</span><span class="sxs-lookup"><span data-stu-id="e35cf-117">The list of school sourcedIds to sync.</span></span> |
| <span data-ttu-id="e35cf-118">**providerName**</span><span class="sxs-lookup"><span data-stu-id="e35cf-118">**providerName**</span></span> | <span data-ttu-id="e35cf-119">字符串</span><span class="sxs-lookup"><span data-stu-id="e35cf-119">String</span></span> | <span data-ttu-id="e35cf-120">由[OneRoster 规范](https://www.imsglobal.org/oneroster-v11-final-best-practice-and-implementation-guide#AppA)定义 OneRoster 服务提供商的名称。</span><span class="sxs-lookup"><span data-stu-id="e35cf-120">The OneRoster Service Provider name as defined by the [OneRoster specification](https://www.imsglobal.org/oneroster-v11-final-best-practice-and-implementation-guide#AppA).</span></span> |
| <span data-ttu-id="e35cf-121">**connectionSettings**</span><span class="sxs-lookup"><span data-stu-id="e35cf-121">**connectionSettings**</span></span> | [<span data-ttu-id="e35cf-122">educationSynchronizationConnectionSettings</span><span class="sxs-lookup"><span data-stu-id="e35cf-122">educationSynchronizationConnectionSettings</span></span>](educationsynchronizationconnectionsettings.md) | <span data-ttu-id="e35cf-123">OneRoster 实例的连接设置。</span><span class="sxs-lookup"><span data-stu-id="e35cf-123">Connection settings for the OneRoster instance.</span></span> <span data-ttu-id="e35cf-124">应类型[educationSynchronizationOAuth1ConnectionSettings](educationsynchronizationoauth1connectionsettings.md)或[educationSynchronizationOAuth2ClientCredentialsConnectionSettings](educationsynchronizationoauth2clientcredentialsconnectionsettings.md)。</span><span class="sxs-lookup"><span data-stu-id="e35cf-124">Should be of type [educationSynchronizationOAuth1ConnectionSettings](educationsynchronizationoauth1connectionsettings.md) or [educationSynchronizationOAuth2ClientCredentialsConnectionSettings](educationsynchronizationoauth2clientcredentialsconnectionsettings.md).</span></span> |
| <span data-ttu-id="e35cf-125">**自定义项**</span><span class="sxs-lookup"><span data-stu-id="e35cf-125">**customizations**</span></span> | [<span data-ttu-id="e35cf-126">educationSynchronizationCustomizations</span><span class="sxs-lookup"><span data-stu-id="e35cf-126">educationSynchronizationCustomizations</span></span>](educationsynchronizationcustomizations.md) | <span data-ttu-id="e35cf-127">可选自定义要应用于同步配置文件。</span><span class="sxs-lookup"><span data-stu-id="e35cf-127">Optional customization to be applied to the synchronization profile.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="e35cf-128">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="e35cf-128">JSON representation</span></span>
<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "#microsoft.graph.educationoneRosterApiDataProvider"
}-->

```json
{
    "@odata.type": "#microsoft.graph.educationoneRosterApiDataProvider",
    "connectionUrl": "String",
    "providerName": "String",
    "schoolsIds": [
        "String"
    ],
    "connectionSettings": {
        "@odata.type": "#microsoft.graph.educationSynchronizationOAuth1ConnectionSettings",
        "clientId": "String",
        "clientSecret": "String",
    },
    "customizations": { "@odata.type": "microsoft.graph.educationSynchronizationCustomizations" }
}
```
