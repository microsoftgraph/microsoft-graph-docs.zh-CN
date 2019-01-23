---
title: certificateConnectorSetting 资源类型
description: 证书连接器设置。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 5886418aaddede43f2397ad626028598a63a0066
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29398651"
---
# <a name="certificateconnectorsetting-resource-type"></a><span data-ttu-id="70c77-103">certificateConnectorSetting 资源类型</span><span class="sxs-lookup"><span data-stu-id="70c77-103">certificateConnectorSetting resource type</span></span>

> <span data-ttu-id="70c77-104">**重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。</span><span class="sxs-lookup"><span data-stu-id="70c77-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="70c77-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="70c77-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="70c77-106">**注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="70c77-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="70c77-107">证书连接器设置。</span><span class="sxs-lookup"><span data-stu-id="70c77-107">Certificate connector settings.</span></span>

## <a name="properties"></a><span data-ttu-id="70c77-108">属性</span><span class="sxs-lookup"><span data-stu-id="70c77-108">Properties</span></span>
|<span data-ttu-id="70c77-109">属性</span><span class="sxs-lookup"><span data-stu-id="70c77-109">Property</span></span>|<span data-ttu-id="70c77-110">类型</span><span class="sxs-lookup"><span data-stu-id="70c77-110">Type</span></span>|<span data-ttu-id="70c77-111">说明</span><span class="sxs-lookup"><span data-stu-id="70c77-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="70c77-112">状态</span><span class="sxs-lookup"><span data-stu-id="70c77-112">status</span></span>|<span data-ttu-id="70c77-113">Int32</span><span class="sxs-lookup"><span data-stu-id="70c77-113">Int32</span></span>|<span data-ttu-id="70c77-114">证书连接器状态</span><span class="sxs-lookup"><span data-stu-id="70c77-114">Certificate connector status</span></span>|
|<span data-ttu-id="70c77-115">certExpiryTime</span><span class="sxs-lookup"><span data-stu-id="70c77-115">certExpiryTime</span></span>|<span data-ttu-id="70c77-116">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="70c77-116">DateTimeOffset</span></span>|<span data-ttu-id="70c77-117">证书过期时间</span><span class="sxs-lookup"><span data-stu-id="70c77-117">Certificate expire time</span></span>|
|<span data-ttu-id="70c77-118">enrollmentError</span><span class="sxs-lookup"><span data-stu-id="70c77-118">enrollmentError</span></span>|<span data-ttu-id="70c77-119">String</span><span class="sxs-lookup"><span data-stu-id="70c77-119">String</span></span>|<span data-ttu-id="70c77-120">证书连接器注册错误</span><span class="sxs-lookup"><span data-stu-id="70c77-120">Certificate connector enrollment error</span></span>|
|<span data-ttu-id="70c77-121">lastConnectorConnectionTime</span><span class="sxs-lookup"><span data-stu-id="70c77-121">lastConnectorConnectionTime</span></span>|<span data-ttu-id="70c77-122">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="70c77-122">DateTimeOffset</span></span>|<span data-ttu-id="70c77-123">最后一次证书连接符连接</span><span class="sxs-lookup"><span data-stu-id="70c77-123">Last time certificate connector connected</span></span>|
|<span data-ttu-id="70c77-124">connectorVersion</span><span class="sxs-lookup"><span data-stu-id="70c77-124">connectorVersion</span></span>|<span data-ttu-id="70c77-125">String</span><span class="sxs-lookup"><span data-stu-id="70c77-125">String</span></span>|<span data-ttu-id="70c77-126">证书连接器的版本</span><span class="sxs-lookup"><span data-stu-id="70c77-126">Version of certificate connector</span></span>|
|<span data-ttu-id="70c77-127">lastUploadVersion</span><span class="sxs-lookup"><span data-stu-id="70c77-127">lastUploadVersion</span></span>|<span data-ttu-id="70c77-128">Int64</span><span class="sxs-lookup"><span data-stu-id="70c77-128">Int64</span></span>|<span data-ttu-id="70c77-129">版本的最后一个上载的证书连接器</span><span class="sxs-lookup"><span data-stu-id="70c77-129">Version of last uploaded certificate connector</span></span>|

## <a name="relationships"></a><span data-ttu-id="70c77-130">关系</span><span class="sxs-lookup"><span data-stu-id="70c77-130">Relationships</span></span>
<span data-ttu-id="70c77-131">无</span><span class="sxs-lookup"><span data-stu-id="70c77-131">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="70c77-132">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="70c77-132">JSON Representation</span></span>
<span data-ttu-id="70c77-133">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="70c77-133">Here is a JSON representation of the resource.</span></span>
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




