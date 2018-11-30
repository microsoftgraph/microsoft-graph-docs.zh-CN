---
title: certificateConnectorSetting 资源类型
description: 证书连接器设置。
ms.openlocfilehash: 65f87002016c4d5bd6b19106ba1aa988ad30d92e
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27041235"
---
# <a name="certificateconnectorsetting-resource-type"></a><span data-ttu-id="e7e08-103">certificateConnectorSetting 资源类型</span><span class="sxs-lookup"><span data-stu-id="e7e08-103">certificateConnectorSetting resource type</span></span>

> <span data-ttu-id="e7e08-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="e7e08-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="e7e08-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="e7e08-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="e7e08-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="e7e08-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="e7e08-107">证书连接器设置。</span><span class="sxs-lookup"><span data-stu-id="e7e08-107">Certificate connector settings.</span></span>
## <a name="properties"></a><span data-ttu-id="e7e08-108">属性</span><span class="sxs-lookup"><span data-stu-id="e7e08-108">Properties</span></span>
|<span data-ttu-id="e7e08-109">属性</span><span class="sxs-lookup"><span data-stu-id="e7e08-109">Property</span></span>|<span data-ttu-id="e7e08-110">类型</span><span class="sxs-lookup"><span data-stu-id="e7e08-110">Type</span></span>|<span data-ttu-id="e7e08-111">说明</span><span class="sxs-lookup"><span data-stu-id="e7e08-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e7e08-112">状态</span><span class="sxs-lookup"><span data-stu-id="e7e08-112">status</span></span>|<span data-ttu-id="e7e08-113">Int32</span><span class="sxs-lookup"><span data-stu-id="e7e08-113">Int32</span></span>|<span data-ttu-id="e7e08-114">证书连接器状态</span><span class="sxs-lookup"><span data-stu-id="e7e08-114">Certificate connector status</span></span>|
|<span data-ttu-id="e7e08-115">certExpiryTime</span><span class="sxs-lookup"><span data-stu-id="e7e08-115">certExpiryTime</span></span>|<span data-ttu-id="e7e08-116">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e7e08-116">DateTimeOffset</span></span>|<span data-ttu-id="e7e08-117">证书过期时间</span><span class="sxs-lookup"><span data-stu-id="e7e08-117">Certificate expire time</span></span>|
|<span data-ttu-id="e7e08-118">enrollmentError</span><span class="sxs-lookup"><span data-stu-id="e7e08-118">enrollmentError</span></span>|<span data-ttu-id="e7e08-119">字符串</span><span class="sxs-lookup"><span data-stu-id="e7e08-119">String</span></span>|<span data-ttu-id="e7e08-120">证书连接器注册错误</span><span class="sxs-lookup"><span data-stu-id="e7e08-120">Certificate connector enrollment error</span></span>|
|<span data-ttu-id="e7e08-121">lastConnectorConnectionTime</span><span class="sxs-lookup"><span data-stu-id="e7e08-121">lastConnectorConnectionTime</span></span>|<span data-ttu-id="e7e08-122">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e7e08-122">DateTimeOffset</span></span>|<span data-ttu-id="e7e08-123">最后一次证书连接符连接</span><span class="sxs-lookup"><span data-stu-id="e7e08-123">Last time certificate connector connected</span></span>|
|<span data-ttu-id="e7e08-124">connectorVersion</span><span class="sxs-lookup"><span data-stu-id="e7e08-124">connectorVersion</span></span>|<span data-ttu-id="e7e08-125">字符串</span><span class="sxs-lookup"><span data-stu-id="e7e08-125">String</span></span>|<span data-ttu-id="e7e08-126">证书连接器的版本</span><span class="sxs-lookup"><span data-stu-id="e7e08-126">Version of certificate connector</span></span>|
|<span data-ttu-id="e7e08-127">lastUploadVersion</span><span class="sxs-lookup"><span data-stu-id="e7e08-127">lastUploadVersion</span></span>|<span data-ttu-id="e7e08-128">Int64</span><span class="sxs-lookup"><span data-stu-id="e7e08-128">Int64</span></span>|<span data-ttu-id="e7e08-129">版本的最后一个上载的证书连接器</span><span class="sxs-lookup"><span data-stu-id="e7e08-129">Version of last uploaded certificate connector</span></span>|

## <a name="relationships"></a><span data-ttu-id="e7e08-130">Relationships</span><span class="sxs-lookup"><span data-stu-id="e7e08-130">Relationships</span></span>
<span data-ttu-id="e7e08-131">无</span><span class="sxs-lookup"><span data-stu-id="e7e08-131">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="e7e08-132">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="e7e08-132">JSON Representation</span></span>
<span data-ttu-id="e7e08-133">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="e7e08-133">Here is a JSON representation of the resource.</span></span>
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





