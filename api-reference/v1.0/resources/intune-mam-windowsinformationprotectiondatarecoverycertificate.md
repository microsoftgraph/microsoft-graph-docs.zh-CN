---
title: windowsInformationProtectionDataRecoveryCertificate 资源类型
description: Windows 信息保护 DataRecoveryCertificate
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 555cac098d2796f612054f11e2c5ade525ad6199
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "36037728"
---
# <a name="windowsinformationprotectiondatarecoverycertificate-resource-type"></a><span data-ttu-id="4abf7-103">windowsInformationProtectionDataRecoveryCertificate 资源类型</span><span class="sxs-lookup"><span data-stu-id="4abf7-103">windowsInformationProtectionDataRecoveryCertificate resource type</span></span>

> <span data-ttu-id="4abf7-104">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="4abf7-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4abf7-105">Windows 信息保护 DataRecoveryCertificate</span><span class="sxs-lookup"><span data-stu-id="4abf7-105">Windows Information Protection DataRecoveryCertificate</span></span>

## <a name="properties"></a><span data-ttu-id="4abf7-106">属性</span><span class="sxs-lookup"><span data-stu-id="4abf7-106">Properties</span></span>
|<span data-ttu-id="4abf7-107">属性</span><span class="sxs-lookup"><span data-stu-id="4abf7-107">Property</span></span>|<span data-ttu-id="4abf7-108">类型</span><span class="sxs-lookup"><span data-stu-id="4abf7-108">Type</span></span>|<span data-ttu-id="4abf7-109">说明</span><span class="sxs-lookup"><span data-stu-id="4abf7-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4abf7-110">SubjectName</span><span class="sxs-lookup"><span data-stu-id="4abf7-110">subjectName</span></span>|<span data-ttu-id="4abf7-111">String</span><span class="sxs-lookup"><span data-stu-id="4abf7-111">String</span></span>|<span data-ttu-id="4abf7-112">数据恢复证书主题名称</span><span class="sxs-lookup"><span data-stu-id="4abf7-112">Data recovery Certificate subject name</span></span>|
|<span data-ttu-id="4abf7-113">说明</span><span class="sxs-lookup"><span data-stu-id="4abf7-113">description</span></span>|<span data-ttu-id="4abf7-114">String</span><span class="sxs-lookup"><span data-stu-id="4abf7-114">String</span></span>|<span data-ttu-id="4abf7-115">数据恢复证书说明</span><span class="sxs-lookup"><span data-stu-id="4abf7-115">Data recovery Certificate description</span></span>|
|<span data-ttu-id="4abf7-116">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="4abf7-116">expirationDateTime</span></span>|<span data-ttu-id="4abf7-117">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4abf7-117">DateTimeOffset</span></span>|<span data-ttu-id="4abf7-118">数据恢复证书过期日期/时间</span><span class="sxs-lookup"><span data-stu-id="4abf7-118">Data recovery Certificate expiration datetime</span></span>|
|<span data-ttu-id="4abf7-119">证书</span><span class="sxs-lookup"><span data-stu-id="4abf7-119">certificate</span></span>|<span data-ttu-id="4abf7-120">Binary</span><span class="sxs-lookup"><span data-stu-id="4abf7-120">Binary</span></span>|<span data-ttu-id="4abf7-121">数据恢复证书</span><span class="sxs-lookup"><span data-stu-id="4abf7-121">Data recovery Certificate</span></span>|

## <a name="relationships"></a><span data-ttu-id="4abf7-122">关系</span><span class="sxs-lookup"><span data-stu-id="4abf7-122">Relationships</span></span>
<span data-ttu-id="4abf7-123">无</span><span class="sxs-lookup"><span data-stu-id="4abf7-123">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="4abf7-124">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="4abf7-124">JSON Representation</span></span>
<span data-ttu-id="4abf7-125">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="4abf7-125">Here is a JSON representation of the resource.</span></span>
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



