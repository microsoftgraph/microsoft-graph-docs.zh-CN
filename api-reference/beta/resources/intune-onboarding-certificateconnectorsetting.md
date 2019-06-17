---
title: certificateConnectorSetting 资源类型
description: 证书连接器设置。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 014d9ab627d1606d9850548128c51ed52939f2c8
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/14/2019
ms.locfileid: "34995537"
---
# <a name="certificateconnectorsetting-resource-type"></a><span data-ttu-id="b2817-103">certificateConnectorSetting 资源类型</span><span class="sxs-lookup"><span data-stu-id="b2817-103">certificateConnectorSetting resource type</span></span>

> <span data-ttu-id="b2817-104">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="b2817-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b2817-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="b2817-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b2817-106">证书连接器设置。</span><span class="sxs-lookup"><span data-stu-id="b2817-106">Certificate connector settings.</span></span>

## <a name="properties"></a><span data-ttu-id="b2817-107">属性</span><span class="sxs-lookup"><span data-stu-id="b2817-107">Properties</span></span>
|<span data-ttu-id="b2817-108">属性</span><span class="sxs-lookup"><span data-stu-id="b2817-108">Property</span></span>|<span data-ttu-id="b2817-109">类型</span><span class="sxs-lookup"><span data-stu-id="b2817-109">Type</span></span>|<span data-ttu-id="b2817-110">说明</span><span class="sxs-lookup"><span data-stu-id="b2817-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b2817-111">状态</span><span class="sxs-lookup"><span data-stu-id="b2817-111">status</span></span>|<span data-ttu-id="b2817-112">Int32</span><span class="sxs-lookup"><span data-stu-id="b2817-112">Int32</span></span>|<span data-ttu-id="b2817-113">证书连接器状态</span><span class="sxs-lookup"><span data-stu-id="b2817-113">Certificate connector status</span></span>|
|<span data-ttu-id="b2817-114">certExpiryTime</span><span class="sxs-lookup"><span data-stu-id="b2817-114">certExpiryTime</span></span>|<span data-ttu-id="b2817-115">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b2817-115">DateTimeOffset</span></span>|<span data-ttu-id="b2817-116">证书过期时间</span><span class="sxs-lookup"><span data-stu-id="b2817-116">Certificate expire time</span></span>|
|<span data-ttu-id="b2817-117">enrollmentError</span><span class="sxs-lookup"><span data-stu-id="b2817-117">enrollmentError</span></span>|<span data-ttu-id="b2817-118">String</span><span class="sxs-lookup"><span data-stu-id="b2817-118">String</span></span>|<span data-ttu-id="b2817-119">证书连接器注册错误</span><span class="sxs-lookup"><span data-stu-id="b2817-119">Certificate connector enrollment error</span></span>|
|<span data-ttu-id="b2817-120">lastConnectorConnectionTime</span><span class="sxs-lookup"><span data-stu-id="b2817-120">lastConnectorConnectionTime</span></span>|<span data-ttu-id="b2817-121">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b2817-121">DateTimeOffset</span></span>|<span data-ttu-id="b2817-122">上次连接证书连接器的时间</span><span class="sxs-lookup"><span data-stu-id="b2817-122">Last time certificate connector connected</span></span>|
|<span data-ttu-id="b2817-123">connectorVersion</span><span class="sxs-lookup"><span data-stu-id="b2817-123">connectorVersion</span></span>|<span data-ttu-id="b2817-124">String</span><span class="sxs-lookup"><span data-stu-id="b2817-124">String</span></span>|<span data-ttu-id="b2817-125">证书连接器的版本</span><span class="sxs-lookup"><span data-stu-id="b2817-125">Version of certificate connector</span></span>|
|<span data-ttu-id="b2817-126">lastUploadVersion</span><span class="sxs-lookup"><span data-stu-id="b2817-126">lastUploadVersion</span></span>|<span data-ttu-id="b2817-127">Int64</span><span class="sxs-lookup"><span data-stu-id="b2817-127">Int64</span></span>|<span data-ttu-id="b2817-128">上次上载的证书连接器的版本</span><span class="sxs-lookup"><span data-stu-id="b2817-128">Version of last uploaded certificate connector</span></span>|

## <a name="relationships"></a><span data-ttu-id="b2817-129">关系</span><span class="sxs-lookup"><span data-stu-id="b2817-129">Relationships</span></span>
<span data-ttu-id="b2817-130">无</span><span class="sxs-lookup"><span data-stu-id="b2817-130">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="b2817-131">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="b2817-131">JSON Representation</span></span>
<span data-ttu-id="b2817-132">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="b2817-132">Here is a JSON representation of the resource.</span></span>
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





