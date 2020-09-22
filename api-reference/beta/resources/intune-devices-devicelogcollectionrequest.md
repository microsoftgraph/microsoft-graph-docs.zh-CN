---
title: deviceLogCollectionRequest 资源类型
description: Windows 日志集合请求实体。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: f6da733d7ba4ff8de8a4110473006806ed0d08de
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48060179"
---
# <a name="devicelogcollectionrequest-resource-type"></a><span data-ttu-id="6d7ec-103">deviceLogCollectionRequest 资源类型</span><span class="sxs-lookup"><span data-stu-id="6d7ec-103">deviceLogCollectionRequest resource type</span></span>

<span data-ttu-id="6d7ec-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6d7ec-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="6d7ec-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="6d7ec-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="6d7ec-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="6d7ec-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6d7ec-107">Windows 日志集合请求实体。</span><span class="sxs-lookup"><span data-stu-id="6d7ec-107">Windows Log Collection request entity.</span></span>

## <a name="properties"></a><span data-ttu-id="6d7ec-108">属性</span><span class="sxs-lookup"><span data-stu-id="6d7ec-108">Properties</span></span>
|<span data-ttu-id="6d7ec-109">属性</span><span class="sxs-lookup"><span data-stu-id="6d7ec-109">Property</span></span>|<span data-ttu-id="6d7ec-110">类型</span><span class="sxs-lookup"><span data-stu-id="6d7ec-110">Type</span></span>|<span data-ttu-id="6d7ec-111">说明</span><span class="sxs-lookup"><span data-stu-id="6d7ec-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6d7ec-112">id</span><span class="sxs-lookup"><span data-stu-id="6d7ec-112">id</span></span>|<span data-ttu-id="6d7ec-113">String</span><span class="sxs-lookup"><span data-stu-id="6d7ec-113">String</span></span>|<span data-ttu-id="6d7ec-114">唯一标识符</span><span class="sxs-lookup"><span data-stu-id="6d7ec-114">The unique identifier</span></span>|
|<span data-ttu-id="6d7ec-115">templateType</span><span class="sxs-lookup"><span data-stu-id="6d7ec-115">templateType</span></span>|[<span data-ttu-id="6d7ec-116">deviceLogCollectionTemplateType</span><span class="sxs-lookup"><span data-stu-id="6d7ec-116">deviceLogCollectionTemplateType</span></span>](../resources/intune-devices-devicelogcollectiontemplatetype.md)|<span data-ttu-id="6d7ec-117">与集合请求一起发送的模板类型。</span><span class="sxs-lookup"><span data-stu-id="6d7ec-117">The template type that is sent with the collection request.</span></span> <span data-ttu-id="6d7ec-118">可能的值是： `predefined` 。</span><span class="sxs-lookup"><span data-stu-id="6d7ec-118">Possible values are: `predefined`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="6d7ec-119">关系</span><span class="sxs-lookup"><span data-stu-id="6d7ec-119">Relationships</span></span>
<span data-ttu-id="6d7ec-120">无</span><span class="sxs-lookup"><span data-stu-id="6d7ec-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="6d7ec-121">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="6d7ec-121">JSON Representation</span></span>
<span data-ttu-id="6d7ec-122">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="6d7ec-122">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceLogCollectionRequest"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceLogCollectionRequest",
  "id": "String (identifier)",
  "templateType": "String"
}
```






