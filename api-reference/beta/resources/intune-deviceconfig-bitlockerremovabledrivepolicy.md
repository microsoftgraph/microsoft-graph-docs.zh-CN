---
title: bitLockerRemovableDrivePolicy 资源类型
description: BitLocker 可移动驱动器策略。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 57a3ad19e988327e126b6da757c2dc5b90c280de
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29425615"
---
# <a name="bitlockerremovabledrivepolicy-resource-type"></a><span data-ttu-id="4ca18-103">bitLockerRemovableDrivePolicy 资源类型</span><span class="sxs-lookup"><span data-stu-id="4ca18-103">bitLockerRemovableDrivePolicy resource type</span></span>

> <span data-ttu-id="4ca18-104">**重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。</span><span class="sxs-lookup"><span data-stu-id="4ca18-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="4ca18-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="4ca18-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="4ca18-106">**注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="4ca18-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4ca18-107">BitLocker 可移动驱动器策略。</span><span class="sxs-lookup"><span data-stu-id="4ca18-107">BitLocker Removable Drive Policies.</span></span>

## <a name="properties"></a><span data-ttu-id="4ca18-108">属性</span><span class="sxs-lookup"><span data-stu-id="4ca18-108">Properties</span></span>
|<span data-ttu-id="4ca18-109">属性</span><span class="sxs-lookup"><span data-stu-id="4ca18-109">Property</span></span>|<span data-ttu-id="4ca18-110">类型</span><span class="sxs-lookup"><span data-stu-id="4ca18-110">Type</span></span>|<span data-ttu-id="4ca18-111">说明</span><span class="sxs-lookup"><span data-stu-id="4ca18-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4ca18-112">encryptionMethod</span><span class="sxs-lookup"><span data-stu-id="4ca18-112">encryptionMethod</span></span>|[<span data-ttu-id="4ca18-113">bitLockerEncryptionMethod</span><span class="sxs-lookup"><span data-stu-id="4ca18-113">bitLockerEncryptionMethod</span></span>](../resources/intune-deviceconfig-bitlockerencryptionmethod.md)|<span data-ttu-id="4ca18-114">选择可移动驱动器的加密方法。</span><span class="sxs-lookup"><span data-stu-id="4ca18-114">Select the encryption method for removable  drives.</span></span> <span data-ttu-id="4ca18-115">可取值为：`aesCbc128`、`aesCbc256`、`xtsAes128`、`xtsAes256`</span><span class="sxs-lookup"><span data-stu-id="4ca18-115">Possible values are: `aesCbc128`, `aesCbc256`, `xtsAes128`, `xtsAes256`.</span></span>|
|<span data-ttu-id="4ca18-116">requireEncryptionForWriteAccess</span><span class="sxs-lookup"><span data-stu-id="4ca18-116">requireEncryptionForWriteAccess</span></span>|<span data-ttu-id="4ca18-117">Boolean</span><span class="sxs-lookup"><span data-stu-id="4ca18-117">Boolean</span></span>|<span data-ttu-id="4ca18-118">指示是否阻止对其他组织中配置的设备的写入权限。</span><span class="sxs-lookup"><span data-stu-id="4ca18-118">Indicates whether to block write access to devices configured in another organization.</span></span>  <span data-ttu-id="4ca18-119">如果 requireEncryptionForWriteAccess 为 false，则此值没有影响。</span><span class="sxs-lookup"><span data-stu-id="4ca18-119">If requireEncryptionForWriteAccess is false, this value does not affect.</span></span>|
|<span data-ttu-id="4ca18-120">blockCrossOrganizationWriteAccess</span><span class="sxs-lookup"><span data-stu-id="4ca18-120">blockCrossOrganizationWriteAccess</span></span>|<span data-ttu-id="4ca18-121">Boolean</span><span class="sxs-lookup"><span data-stu-id="4ca18-121">Boolean</span></span>|<span data-ttu-id="4ca18-122">此策略设置决定可移动数据驱动器是否需要 BitLocker 保护，以使其在计算机上可写。</span><span class="sxs-lookup"><span data-stu-id="4ca18-122">This policy setting determines whether BitLocker protection is required for removable data drives to be writable on a computer.</span></span>|

## <a name="relationships"></a><span data-ttu-id="4ca18-123">关系</span><span class="sxs-lookup"><span data-stu-id="4ca18-123">Relationships</span></span>
<span data-ttu-id="4ca18-124">无</span><span class="sxs-lookup"><span data-stu-id="4ca18-124">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="4ca18-125">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="4ca18-125">JSON Representation</span></span>
<span data-ttu-id="4ca18-126">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="4ca18-126">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.bitLockerRemovableDrivePolicy"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.bitLockerRemovableDrivePolicy",
  "encryptionMethod": "String",
  "requireEncryptionForWriteAccess": true,
  "blockCrossOrganizationWriteAccess": true
}
```




