---
title: certificateConnectorSetting 资源类型
description: 证书连接器设置。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 2b69643b20d02b23d70c6f3425a4b2422c69ee86
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2020
ms.locfileid: "49288192"
---
# <a name="certificateconnectorsetting-resource-type"></a><span data-ttu-id="8bc23-103">certificateConnectorSetting 资源类型</span><span class="sxs-lookup"><span data-stu-id="8bc23-103">certificateConnectorSetting resource type</span></span>

<span data-ttu-id="8bc23-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8bc23-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="8bc23-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="8bc23-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="8bc23-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="8bc23-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8bc23-107">证书连接器设置。</span><span class="sxs-lookup"><span data-stu-id="8bc23-107">Certificate connector settings.</span></span>

## <a name="properties"></a><span data-ttu-id="8bc23-108">属性</span><span class="sxs-lookup"><span data-stu-id="8bc23-108">Properties</span></span>
|<span data-ttu-id="8bc23-109">属性</span><span class="sxs-lookup"><span data-stu-id="8bc23-109">Property</span></span>|<span data-ttu-id="8bc23-110">类型</span><span class="sxs-lookup"><span data-stu-id="8bc23-110">Type</span></span>|<span data-ttu-id="8bc23-111">Description</span><span class="sxs-lookup"><span data-stu-id="8bc23-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8bc23-112">状态</span><span class="sxs-lookup"><span data-stu-id="8bc23-112">status</span></span>|<span data-ttu-id="8bc23-113">Int32</span><span class="sxs-lookup"><span data-stu-id="8bc23-113">Int32</span></span>|<span data-ttu-id="8bc23-114">证书连接器状态</span><span class="sxs-lookup"><span data-stu-id="8bc23-114">Certificate connector status</span></span>|
|<span data-ttu-id="8bc23-115">certExpiryTime</span><span class="sxs-lookup"><span data-stu-id="8bc23-115">certExpiryTime</span></span>|<span data-ttu-id="8bc23-116">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8bc23-116">DateTimeOffset</span></span>|<span data-ttu-id="8bc23-117">证书过期时间</span><span class="sxs-lookup"><span data-stu-id="8bc23-117">Certificate expire time</span></span>|
|<span data-ttu-id="8bc23-118">enrollmentError</span><span class="sxs-lookup"><span data-stu-id="8bc23-118">enrollmentError</span></span>|<span data-ttu-id="8bc23-119">字符串</span><span class="sxs-lookup"><span data-stu-id="8bc23-119">String</span></span>|<span data-ttu-id="8bc23-120">证书连接器注册错误</span><span class="sxs-lookup"><span data-stu-id="8bc23-120">Certificate connector enrollment error</span></span>|
|<span data-ttu-id="8bc23-121">lastConnectorConnectionTime</span><span class="sxs-lookup"><span data-stu-id="8bc23-121">lastConnectorConnectionTime</span></span>|<span data-ttu-id="8bc23-122">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8bc23-122">DateTimeOffset</span></span>|<span data-ttu-id="8bc23-123">上次连接证书连接器的时间</span><span class="sxs-lookup"><span data-stu-id="8bc23-123">Last time certificate connector connected</span></span>|
|<span data-ttu-id="8bc23-124">connectorVersion</span><span class="sxs-lookup"><span data-stu-id="8bc23-124">connectorVersion</span></span>|<span data-ttu-id="8bc23-125">字符串</span><span class="sxs-lookup"><span data-stu-id="8bc23-125">String</span></span>|<span data-ttu-id="8bc23-126">证书连接器的版本</span><span class="sxs-lookup"><span data-stu-id="8bc23-126">Version of certificate connector</span></span>|
|<span data-ttu-id="8bc23-127">lastUploadVersion</span><span class="sxs-lookup"><span data-stu-id="8bc23-127">lastUploadVersion</span></span>|<span data-ttu-id="8bc23-128">Int64</span><span class="sxs-lookup"><span data-stu-id="8bc23-128">Int64</span></span>|<span data-ttu-id="8bc23-129">上次上载的证书连接器的版本</span><span class="sxs-lookup"><span data-stu-id="8bc23-129">Version of last uploaded certificate connector</span></span>|

## <a name="relationships"></a><span data-ttu-id="8bc23-130">关系</span><span class="sxs-lookup"><span data-stu-id="8bc23-130">Relationships</span></span>
<span data-ttu-id="8bc23-131">无</span><span class="sxs-lookup"><span data-stu-id="8bc23-131">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="8bc23-132">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="8bc23-132">JSON Representation</span></span>
<span data-ttu-id="8bc23-133">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="8bc23-133">Here is a JSON representation of the resource.</span></span>
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




