---
title: windowsInformationProtectionDataRecoveryCertificate 资源类型
description: Windows 信息保护 DataRecoveryCertificate
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: fce6d146e267d0b64d1f95cf15e23b92e6e33720
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/14/2020
ms.locfileid: "43468426"
---
# <a name="windowsinformationprotectiondatarecoverycertificate-resource-type"></a><span data-ttu-id="3d3ca-103">windowsInformationProtectionDataRecoveryCertificate 资源类型</span><span class="sxs-lookup"><span data-stu-id="3d3ca-103">windowsInformationProtectionDataRecoveryCertificate resource type</span></span>

<span data-ttu-id="3d3ca-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3d3ca-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="3d3ca-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="3d3ca-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3d3ca-106">Windows 信息保护 DataRecoveryCertificate</span><span class="sxs-lookup"><span data-stu-id="3d3ca-106">Windows Information Protection DataRecoveryCertificate</span></span>

## <a name="properties"></a><span data-ttu-id="3d3ca-107">属性</span><span class="sxs-lookup"><span data-stu-id="3d3ca-107">Properties</span></span>
|<span data-ttu-id="3d3ca-108">属性</span><span class="sxs-lookup"><span data-stu-id="3d3ca-108">Property</span></span>|<span data-ttu-id="3d3ca-109">类型</span><span class="sxs-lookup"><span data-stu-id="3d3ca-109">Type</span></span>|<span data-ttu-id="3d3ca-110">说明</span><span class="sxs-lookup"><span data-stu-id="3d3ca-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3d3ca-111">SubjectName</span><span class="sxs-lookup"><span data-stu-id="3d3ca-111">subjectName</span></span>|<span data-ttu-id="3d3ca-112">String</span><span class="sxs-lookup"><span data-stu-id="3d3ca-112">String</span></span>|<span data-ttu-id="3d3ca-113">数据恢复证书主题名称</span><span class="sxs-lookup"><span data-stu-id="3d3ca-113">Data recovery Certificate subject name</span></span>|
|<span data-ttu-id="3d3ca-114">description</span><span class="sxs-lookup"><span data-stu-id="3d3ca-114">description</span></span>|<span data-ttu-id="3d3ca-115">String</span><span class="sxs-lookup"><span data-stu-id="3d3ca-115">String</span></span>|<span data-ttu-id="3d3ca-116">数据恢复证书说明</span><span class="sxs-lookup"><span data-stu-id="3d3ca-116">Data recovery Certificate description</span></span>|
|<span data-ttu-id="3d3ca-117">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="3d3ca-117">expirationDateTime</span></span>|<span data-ttu-id="3d3ca-118">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3d3ca-118">DateTimeOffset</span></span>|<span data-ttu-id="3d3ca-119">数据恢复证书过期日期/时间</span><span class="sxs-lookup"><span data-stu-id="3d3ca-119">Data recovery Certificate expiration datetime</span></span>|
|<span data-ttu-id="3d3ca-120">证书</span><span class="sxs-lookup"><span data-stu-id="3d3ca-120">certificate</span></span>|<span data-ttu-id="3d3ca-121">Binary</span><span class="sxs-lookup"><span data-stu-id="3d3ca-121">Binary</span></span>|<span data-ttu-id="3d3ca-122">数据恢复证书</span><span class="sxs-lookup"><span data-stu-id="3d3ca-122">Data recovery Certificate</span></span>|

## <a name="relationships"></a><span data-ttu-id="3d3ca-123">关系</span><span class="sxs-lookup"><span data-stu-id="3d3ca-123">Relationships</span></span>
<span data-ttu-id="3d3ca-124">无</span><span class="sxs-lookup"><span data-stu-id="3d3ca-124">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="3d3ca-125">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="3d3ca-125">JSON Representation</span></span>
<span data-ttu-id="3d3ca-126">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="3d3ca-126">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.windowsInformationProtectionDataRecoveryCertificate"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsInformationProtectionDataRecoveryCertificate",
  "subjectName": "String",
  "description": "String",
  "expirationDateTime": "String (timestamp)",
  "certificate": "binary"
}
```







