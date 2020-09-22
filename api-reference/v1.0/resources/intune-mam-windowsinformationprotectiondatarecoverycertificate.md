---
title: windowsInformationProtectionDataRecoveryCertificate 资源类型
description: Windows 信息保护 DataRecoveryCertificate
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 1da5da59fb0b3b2485ed2dd22710e13f64307843
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "47984374"
---
# <a name="windowsinformationprotectiondatarecoverycertificate-resource-type"></a><span data-ttu-id="76091-103">windowsInformationProtectionDataRecoveryCertificate 资源类型</span><span class="sxs-lookup"><span data-stu-id="76091-103">windowsInformationProtectionDataRecoveryCertificate resource type</span></span>

<span data-ttu-id="76091-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="76091-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="76091-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="76091-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="76091-106">Windows 信息保护 DataRecoveryCertificate</span><span class="sxs-lookup"><span data-stu-id="76091-106">Windows Information Protection DataRecoveryCertificate</span></span>

## <a name="properties"></a><span data-ttu-id="76091-107">属性</span><span class="sxs-lookup"><span data-stu-id="76091-107">Properties</span></span>
|<span data-ttu-id="76091-108">属性</span><span class="sxs-lookup"><span data-stu-id="76091-108">Property</span></span>|<span data-ttu-id="76091-109">类型</span><span class="sxs-lookup"><span data-stu-id="76091-109">Type</span></span>|<span data-ttu-id="76091-110">说明</span><span class="sxs-lookup"><span data-stu-id="76091-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="76091-111">SubjectName</span><span class="sxs-lookup"><span data-stu-id="76091-111">subjectName</span></span>|<span data-ttu-id="76091-112">String</span><span class="sxs-lookup"><span data-stu-id="76091-112">String</span></span>|<span data-ttu-id="76091-113">数据恢复证书主题名称</span><span class="sxs-lookup"><span data-stu-id="76091-113">Data recovery Certificate subject name</span></span>|
|<span data-ttu-id="76091-114">description</span><span class="sxs-lookup"><span data-stu-id="76091-114">description</span></span>|<span data-ttu-id="76091-115">String</span><span class="sxs-lookup"><span data-stu-id="76091-115">String</span></span>|<span data-ttu-id="76091-116">数据恢复证书说明</span><span class="sxs-lookup"><span data-stu-id="76091-116">Data recovery Certificate description</span></span>|
|<span data-ttu-id="76091-117">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="76091-117">expirationDateTime</span></span>|<span data-ttu-id="76091-118">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="76091-118">DateTimeOffset</span></span>|<span data-ttu-id="76091-119">数据恢复证书过期日期/时间</span><span class="sxs-lookup"><span data-stu-id="76091-119">Data recovery Certificate expiration datetime</span></span>|
|<span data-ttu-id="76091-120">证书</span><span class="sxs-lookup"><span data-stu-id="76091-120">certificate</span></span>|<span data-ttu-id="76091-121">Binary</span><span class="sxs-lookup"><span data-stu-id="76091-121">Binary</span></span>|<span data-ttu-id="76091-122">数据恢复证书</span><span class="sxs-lookup"><span data-stu-id="76091-122">Data recovery Certificate</span></span>|

## <a name="relationships"></a><span data-ttu-id="76091-123">关系</span><span class="sxs-lookup"><span data-stu-id="76091-123">Relationships</span></span>
<span data-ttu-id="76091-124">无</span><span class="sxs-lookup"><span data-stu-id="76091-124">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="76091-125">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="76091-125">JSON Representation</span></span>
<span data-ttu-id="76091-126">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="76091-126">Here is a JSON representation of the resource.</span></span>
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









