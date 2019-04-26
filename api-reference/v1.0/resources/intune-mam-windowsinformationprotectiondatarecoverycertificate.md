---
title: windowsInformationProtectionDataRecoveryCertificate 资源类型
description: Windows 信息保护 DataRecoveryCertificate
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: c321ea06e27e7d6fba0a35446e2b916aaf0689de
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32561185"
---
# <a name="windowsinformationprotectiondatarecoverycertificate-resource-type"></a><span data-ttu-id="3e39a-103">windowsInformationProtectionDataRecoveryCertificate 资源类型</span><span class="sxs-lookup"><span data-stu-id="3e39a-103">windowsInformationProtectionDataRecoveryCertificate resource type</span></span>

> <span data-ttu-id="3e39a-104">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="3e39a-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3e39a-105">Windows 信息保护 DataRecoveryCertificate</span><span class="sxs-lookup"><span data-stu-id="3e39a-105">Windows Information Protection DataRecoveryCertificate</span></span>

## <a name="properties"></a><span data-ttu-id="3e39a-106">属性</span><span class="sxs-lookup"><span data-stu-id="3e39a-106">Properties</span></span>
|<span data-ttu-id="3e39a-107">属性</span><span class="sxs-lookup"><span data-stu-id="3e39a-107">Property</span></span>|<span data-ttu-id="3e39a-108">类型</span><span class="sxs-lookup"><span data-stu-id="3e39a-108">Type</span></span>|<span data-ttu-id="3e39a-109">说明</span><span class="sxs-lookup"><span data-stu-id="3e39a-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3e39a-110">SubjectName</span><span class="sxs-lookup"><span data-stu-id="3e39a-110">subjectName</span></span>|<span data-ttu-id="3e39a-111">String</span><span class="sxs-lookup"><span data-stu-id="3e39a-111">String</span></span>|<span data-ttu-id="3e39a-112">数据恢复证书主题名称</span><span class="sxs-lookup"><span data-stu-id="3e39a-112">Data recovery Certificate subject name</span></span>|
|<span data-ttu-id="3e39a-113">description</span><span class="sxs-lookup"><span data-stu-id="3e39a-113">description</span></span>|<span data-ttu-id="3e39a-114">String</span><span class="sxs-lookup"><span data-stu-id="3e39a-114">String</span></span>|<span data-ttu-id="3e39a-115">数据恢复证书说明</span><span class="sxs-lookup"><span data-stu-id="3e39a-115">Data recovery Certificate description</span></span>|
|<span data-ttu-id="3e39a-116">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="3e39a-116">expirationDateTime</span></span>|<span data-ttu-id="3e39a-117">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3e39a-117">DateTimeOffset</span></span>|<span data-ttu-id="3e39a-118">数据恢复证书过期日期/时间</span><span class="sxs-lookup"><span data-stu-id="3e39a-118">Data recovery Certificate expiration datetime</span></span>|
|<span data-ttu-id="3e39a-119">证书</span><span class="sxs-lookup"><span data-stu-id="3e39a-119">certificate</span></span>|<span data-ttu-id="3e39a-120">Binary</span><span class="sxs-lookup"><span data-stu-id="3e39a-120">Binary</span></span>|<span data-ttu-id="3e39a-121">数据恢复证书</span><span class="sxs-lookup"><span data-stu-id="3e39a-121">Data recovery Certificate</span></span>|

## <a name="relationships"></a><span data-ttu-id="3e39a-122">关系</span><span class="sxs-lookup"><span data-stu-id="3e39a-122">Relationships</span></span>
<span data-ttu-id="3e39a-123">无</span><span class="sxs-lookup"><span data-stu-id="3e39a-123">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="3e39a-124">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="3e39a-124">JSON Representation</span></span>
<span data-ttu-id="3e39a-125">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="3e39a-125">Here is a JSON representation of the resource.</span></span>
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



