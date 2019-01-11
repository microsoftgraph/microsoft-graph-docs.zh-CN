---
title: certificateConnectorSetting 资源类型
description: 证书连接器设置。
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 56f12600b6aa78982dc51732d685dcd7c962d0b0
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27888597"
---
# <a name="certificateconnectorsetting-resource-type"></a><span data-ttu-id="e7bab-103">certificateConnectorSetting 资源类型</span><span class="sxs-lookup"><span data-stu-id="e7bab-103">certificateConnectorSetting resource type</span></span>

> <span data-ttu-id="e7bab-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="e7bab-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="e7bab-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="e7bab-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="e7bab-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="e7bab-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="e7bab-107">证书连接器设置。</span><span class="sxs-lookup"><span data-stu-id="e7bab-107">Certificate connector settings.</span></span>
## <a name="properties"></a><span data-ttu-id="e7bab-108">属性</span><span class="sxs-lookup"><span data-stu-id="e7bab-108">Properties</span></span>
|<span data-ttu-id="e7bab-109">属性</span><span class="sxs-lookup"><span data-stu-id="e7bab-109">Property</span></span>|<span data-ttu-id="e7bab-110">类型</span><span class="sxs-lookup"><span data-stu-id="e7bab-110">Type</span></span>|<span data-ttu-id="e7bab-111">说明</span><span class="sxs-lookup"><span data-stu-id="e7bab-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e7bab-112">状态</span><span class="sxs-lookup"><span data-stu-id="e7bab-112">status</span></span>|<span data-ttu-id="e7bab-113">Int32</span><span class="sxs-lookup"><span data-stu-id="e7bab-113">Int32</span></span>|<span data-ttu-id="e7bab-114">证书连接器状态</span><span class="sxs-lookup"><span data-stu-id="e7bab-114">Certificate connector status</span></span>|
|<span data-ttu-id="e7bab-115">certExpiryTime</span><span class="sxs-lookup"><span data-stu-id="e7bab-115">certExpiryTime</span></span>|<span data-ttu-id="e7bab-116">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e7bab-116">DateTimeOffset</span></span>|<span data-ttu-id="e7bab-117">证书过期时间</span><span class="sxs-lookup"><span data-stu-id="e7bab-117">Certificate expire time</span></span>|
|<span data-ttu-id="e7bab-118">enrollmentError</span><span class="sxs-lookup"><span data-stu-id="e7bab-118">enrollmentError</span></span>|<span data-ttu-id="e7bab-119">字符串</span><span class="sxs-lookup"><span data-stu-id="e7bab-119">String</span></span>|<span data-ttu-id="e7bab-120">证书连接器注册错误</span><span class="sxs-lookup"><span data-stu-id="e7bab-120">Certificate connector enrollment error</span></span>|
|<span data-ttu-id="e7bab-121">lastConnectorConnectionTime</span><span class="sxs-lookup"><span data-stu-id="e7bab-121">lastConnectorConnectionTime</span></span>|<span data-ttu-id="e7bab-122">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e7bab-122">DateTimeOffset</span></span>|<span data-ttu-id="e7bab-123">最后一次证书连接符连接</span><span class="sxs-lookup"><span data-stu-id="e7bab-123">Last time certificate connector connected</span></span>|
|<span data-ttu-id="e7bab-124">connectorVersion</span><span class="sxs-lookup"><span data-stu-id="e7bab-124">connectorVersion</span></span>|<span data-ttu-id="e7bab-125">字符串</span><span class="sxs-lookup"><span data-stu-id="e7bab-125">String</span></span>|<span data-ttu-id="e7bab-126">证书连接器的版本</span><span class="sxs-lookup"><span data-stu-id="e7bab-126">Version of certificate connector</span></span>|
|<span data-ttu-id="e7bab-127">lastUploadVersion</span><span class="sxs-lookup"><span data-stu-id="e7bab-127">lastUploadVersion</span></span>|<span data-ttu-id="e7bab-128">Int64</span><span class="sxs-lookup"><span data-stu-id="e7bab-128">Int64</span></span>|<span data-ttu-id="e7bab-129">版本的最后一个上载的证书连接器</span><span class="sxs-lookup"><span data-stu-id="e7bab-129">Version of last uploaded certificate connector</span></span>|

## <a name="relationships"></a><span data-ttu-id="e7bab-130">Relationships</span><span class="sxs-lookup"><span data-stu-id="e7bab-130">Relationships</span></span>
<span data-ttu-id="e7bab-131">无</span><span class="sxs-lookup"><span data-stu-id="e7bab-131">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="e7bab-132">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="e7bab-132">JSON Representation</span></span>
<span data-ttu-id="e7bab-133">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="e7bab-133">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.certificateConnectorSetting"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.certificateConnectorSetting",
  "status": 1024,
  "certExpiryTime": "String (timestamp)",
  "enrollmentError": "String",
  "lastConnectorConnectionTime": "String (timestamp)",
  "connectorVersion": "String",
  "lastUploadVersion": 1024
}
```





