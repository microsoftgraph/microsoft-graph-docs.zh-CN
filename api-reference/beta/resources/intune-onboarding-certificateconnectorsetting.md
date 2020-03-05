---
title: certificateConnectorSetting 资源类型
description: 证书连接器设置。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 8778bd6b3594ebe1c9a33c2960955e1de63f8cb9
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42524207"
---
# <a name="certificateconnectorsetting-resource-type"></a><span data-ttu-id="ea188-103">certificateConnectorSetting 资源类型</span><span class="sxs-lookup"><span data-stu-id="ea188-103">certificateConnectorSetting resource type</span></span>

<span data-ttu-id="ea188-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="ea188-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="ea188-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="ea188-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ea188-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="ea188-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ea188-107">证书连接器设置。</span><span class="sxs-lookup"><span data-stu-id="ea188-107">Certificate connector settings.</span></span>

## <a name="properties"></a><span data-ttu-id="ea188-108">属性</span><span class="sxs-lookup"><span data-stu-id="ea188-108">Properties</span></span>
|<span data-ttu-id="ea188-109">属性</span><span class="sxs-lookup"><span data-stu-id="ea188-109">Property</span></span>|<span data-ttu-id="ea188-110">类型</span><span class="sxs-lookup"><span data-stu-id="ea188-110">Type</span></span>|<span data-ttu-id="ea188-111">说明</span><span class="sxs-lookup"><span data-stu-id="ea188-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ea188-112">状态</span><span class="sxs-lookup"><span data-stu-id="ea188-112">status</span></span>|<span data-ttu-id="ea188-113">Int32</span><span class="sxs-lookup"><span data-stu-id="ea188-113">Int32</span></span>|<span data-ttu-id="ea188-114">证书连接器状态</span><span class="sxs-lookup"><span data-stu-id="ea188-114">Certificate connector status</span></span>|
|<span data-ttu-id="ea188-115">certExpiryTime</span><span class="sxs-lookup"><span data-stu-id="ea188-115">certExpiryTime</span></span>|<span data-ttu-id="ea188-116">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ea188-116">DateTimeOffset</span></span>|<span data-ttu-id="ea188-117">证书过期时间</span><span class="sxs-lookup"><span data-stu-id="ea188-117">Certificate expire time</span></span>|
|<span data-ttu-id="ea188-118">enrollmentError</span><span class="sxs-lookup"><span data-stu-id="ea188-118">enrollmentError</span></span>|<span data-ttu-id="ea188-119">String</span><span class="sxs-lookup"><span data-stu-id="ea188-119">String</span></span>|<span data-ttu-id="ea188-120">证书连接器注册错误</span><span class="sxs-lookup"><span data-stu-id="ea188-120">Certificate connector enrollment error</span></span>|
|<span data-ttu-id="ea188-121">lastConnectorConnectionTime</span><span class="sxs-lookup"><span data-stu-id="ea188-121">lastConnectorConnectionTime</span></span>|<span data-ttu-id="ea188-122">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ea188-122">DateTimeOffset</span></span>|<span data-ttu-id="ea188-123">上次连接证书连接器的时间</span><span class="sxs-lookup"><span data-stu-id="ea188-123">Last time certificate connector connected</span></span>|
|<span data-ttu-id="ea188-124">connectorVersion</span><span class="sxs-lookup"><span data-stu-id="ea188-124">connectorVersion</span></span>|<span data-ttu-id="ea188-125">String</span><span class="sxs-lookup"><span data-stu-id="ea188-125">String</span></span>|<span data-ttu-id="ea188-126">证书连接器的版本</span><span class="sxs-lookup"><span data-stu-id="ea188-126">Version of certificate connector</span></span>|
|<span data-ttu-id="ea188-127">lastUploadVersion</span><span class="sxs-lookup"><span data-stu-id="ea188-127">lastUploadVersion</span></span>|<span data-ttu-id="ea188-128">Int64</span><span class="sxs-lookup"><span data-stu-id="ea188-128">Int64</span></span>|<span data-ttu-id="ea188-129">上次上载的证书连接器的版本</span><span class="sxs-lookup"><span data-stu-id="ea188-129">Version of last uploaded certificate connector</span></span>|

## <a name="relationships"></a><span data-ttu-id="ea188-130">关系</span><span class="sxs-lookup"><span data-stu-id="ea188-130">Relationships</span></span>
<span data-ttu-id="ea188-131">无</span><span class="sxs-lookup"><span data-stu-id="ea188-131">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="ea188-132">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="ea188-132">JSON Representation</span></span>
<span data-ttu-id="ea188-133">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="ea188-133">Here is a JSON representation of the resource.</span></span>
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



