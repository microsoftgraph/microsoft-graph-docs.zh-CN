---
title: registryKeyState 资源类型
description: 包含有关与警报相关的注册表项更改的信息, 以及更改了注册表项的过程。
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: 672a782b97b3a96c9a7065f3bf5c7b5b9030f282
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "35965451"
---
# <a name="registrykeystate-resource-type"></a><span data-ttu-id="ad307-103">registryKeyState 资源类型</span><span class="sxs-lookup"><span data-stu-id="ad307-103">registryKeyState resource type</span></span>

<span data-ttu-id="ad307-104">包含有关与警报相关的注册表项更改的信息, 以及更改了注册表项的过程。</span><span class="sxs-lookup"><span data-stu-id="ad307-104">Contains information about registry key changes related to the alert, and the process that changed the registry keys.</span></span>

## <a name="properties"></a><span data-ttu-id="ad307-105">属性</span><span class="sxs-lookup"><span data-stu-id="ad307-105">Properties</span></span>

| <span data-ttu-id="ad307-106">属性</span><span class="sxs-lookup"><span data-stu-id="ad307-106">Property</span></span>     | <span data-ttu-id="ad307-107">类型</span><span class="sxs-lookup"><span data-stu-id="ad307-107">Type</span></span>        | <span data-ttu-id="ad307-108">说明</span><span class="sxs-lookup"><span data-stu-id="ad307-108">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="ad307-109">配置单元</span><span class="sxs-lookup"><span data-stu-id="ad307-109">hive</span></span>|<span data-ttu-id="ad307-110">registryHive</span><span class="sxs-lookup"><span data-stu-id="ad307-110">registryHive</span></span>|<span data-ttu-id="ad307-111">[Windows 注册表配置单元](https://docs.microsoft.com/en-us/windows/desktop/sysinfo/registry-hives):</span><span class="sxs-lookup"><span data-stu-id="ad307-111">A [Windows registry hive](https://docs.microsoft.com/en-us/windows/desktop/sysinfo/registry-hives) :</span></span> <ul><li><span data-ttu-id="ad307-112">HKEY_CURRENT_CONFIG</span><span class="sxs-lookup"><span data-stu-id="ad307-112">HKEY_CURRENT_CONFIG</span></span></li> <li><span data-ttu-id="ad307-113">HKEY_CURRENT_USER</span><span class="sxs-lookup"><span data-stu-id="ad307-113">HKEY_CURRENT_USER</span></span></li> <li><span data-ttu-id="ad307-114">HKEY_LOCAL_MACHINE\SAM</span><span class="sxs-lookup"><span data-stu-id="ad307-114">HKEY_LOCAL_MACHINE\SAM</span></span></li> <li><span data-ttu-id="ad307-115">HKEY_LOCAL_MACHINE\Security</span><span class="sxs-lookup"><span data-stu-id="ad307-115">HKEY_LOCAL_MACHINE\Security</span></span></li> <li><span data-ttu-id="ad307-116">HKEY_LOCAL_MACHINE\Software</span><span class="sxs-lookup"><span data-stu-id="ad307-116">HKEY_LOCAL_MACHINE\Software</span></span></li> <li><span data-ttu-id="ad307-117">HKEY_LOCAL_MACHINE\System</span><span class="sxs-lookup"><span data-stu-id="ad307-117">HKEY_LOCAL_MACHINE\System</span></span></li> <li><span data-ttu-id="ad307-118">HKEY_USERS\\。设置.</span><span class="sxs-lookup"><span data-stu-id="ad307-118">HKEY_USERS\\.Default.</span></span></li></ul> <span data-ttu-id="ad307-119">可取值为：`unknown`、`currentConfig`、`currentUser`、`localMachineSam`、`localMachineSecurity`、`localMachineSoftware`、`localMachineSystem`、`usersDefault`。</span><span class="sxs-lookup"><span data-stu-id="ad307-119">Possible values are: `unknown`, `currentConfig`, `currentUser`, `localMachineSam`, `localMachineSecurity`, `localMachineSoftware`, `localMachineSystem`, `usersDefault`.</span></span>|
|<span data-ttu-id="ad307-120">注册表项</span><span class="sxs-lookup"><span data-stu-id="ad307-120">key</span></span>|<span data-ttu-id="ad307-121">String</span><span class="sxs-lookup"><span data-stu-id="ad307-121">String</span></span>|<span data-ttu-id="ad307-122">当前 (如已更改) 的注册表项 (不包括配置单元)。</span><span class="sxs-lookup"><span data-stu-id="ad307-122">Current (i.e. changed) registry key (excludes HIVE).</span></span>|
|<span data-ttu-id="ad307-123">oldKey</span><span class="sxs-lookup"><span data-stu-id="ad307-123">oldKey</span></span>|<span data-ttu-id="ad307-124">String</span><span class="sxs-lookup"><span data-stu-id="ad307-124">String</span></span>|<span data-ttu-id="ad307-125">上一个 (即 "更改前") 注册表项 (不包括 HIVE)。</span><span class="sxs-lookup"><span data-stu-id="ad307-125">Previous (i.e. before changed) registry key (excludes HIVE).</span></span>|
|<span data-ttu-id="ad307-126">oldValueData</span><span class="sxs-lookup"><span data-stu-id="ad307-126">oldValueData</span></span>|<span data-ttu-id="ad307-127">String</span><span class="sxs-lookup"><span data-stu-id="ad307-127">String</span></span>|<span data-ttu-id="ad307-128">以前的 (即更改之前) 注册表项值数据 (内容)。</span><span class="sxs-lookup"><span data-stu-id="ad307-128">Previous (i.e. before changed) registry key value data (contents).</span></span>|
|<span data-ttu-id="ad307-129">oldValueName</span><span class="sxs-lookup"><span data-stu-id="ad307-129">oldValueName</span></span>|<span data-ttu-id="ad307-130">String</span><span class="sxs-lookup"><span data-stu-id="ad307-130">String</span></span>|<span data-ttu-id="ad307-131">以前的注册表项值名称 (即 "更改前")。</span><span class="sxs-lookup"><span data-stu-id="ad307-131">Previous (i.e. before changed) registry key value name.</span></span>|
|<span data-ttu-id="ad307-132">操作</span><span class="sxs-lookup"><span data-stu-id="ad307-132">operation</span></span>|<span data-ttu-id="ad307-133">registryOperation</span><span class="sxs-lookup"><span data-stu-id="ad307-133">registryOperation</span></span>|<span data-ttu-id="ad307-134">更改注册表项名称和/或值的操作。</span><span class="sxs-lookup"><span data-stu-id="ad307-134">Operation that changed the registry key name and/or value.</span></span> <span data-ttu-id="ad307-135">可取值为：`unknown`、`create`、`modify`、`delete`。</span><span class="sxs-lookup"><span data-stu-id="ad307-135">Possible values are: `unknown`, `create`, `modify`, `delete`.</span></span>|
|<span data-ttu-id="ad307-136">processId</span><span class="sxs-lookup"><span data-stu-id="ad307-136">processId</span></span>|<span data-ttu-id="ad307-137">Int32</span><span class="sxs-lookup"><span data-stu-id="ad307-137">Int32</span></span>|<span data-ttu-id="ad307-138">修改注册表项的进程的进程 ID (PID) (进程详细信息将显示在警报的 "进程" 集合中)。</span><span class="sxs-lookup"><span data-stu-id="ad307-138">Process ID (PID) of the process that modified the registry key (process details will appear in the alert 'processes' collection).</span></span>|
|<span data-ttu-id="ad307-139">valueData</span><span class="sxs-lookup"><span data-stu-id="ad307-139">valueData</span></span>|<span data-ttu-id="ad307-140">String</span><span class="sxs-lookup"><span data-stu-id="ad307-140">String</span></span>|<span data-ttu-id="ad307-141">当前 (如已更改) 的注册表项值数据 (内容)。</span><span class="sxs-lookup"><span data-stu-id="ad307-141">Current (i.e. changed) registry key value data (contents).</span></span>|
|<span data-ttu-id="ad307-142">等值</span><span class="sxs-lookup"><span data-stu-id="ad307-142">valueName</span></span>|<span data-ttu-id="ad307-143">String</span><span class="sxs-lookup"><span data-stu-id="ad307-143">String</span></span>|<span data-ttu-id="ad307-144">当前 (如已更改) 的注册表项值名称</span><span class="sxs-lookup"><span data-stu-id="ad307-144">Current (i.e. changed) registry key value name</span></span>|
|<span data-ttu-id="ad307-145">valueType</span><span class="sxs-lookup"><span data-stu-id="ad307-145">valueType</span></span>|<span data-ttu-id="ad307-146">registryValueType</span><span class="sxs-lookup"><span data-stu-id="ad307-146">registryValueType</span></span>|[<span data-ttu-id="ad307-147">注册表项值类型</span><span class="sxs-lookup"><span data-stu-id="ad307-147">Registry key value type</span></span>](https://docs.microsoft.com/en-us/windows/desktop/sysinfo/registry-value-types) <ul><li><span data-ttu-id="ad307-148">REG_BINARY</span><span class="sxs-lookup"><span data-stu-id="ad307-148">REG_BINARY</span></span></li> <li><span data-ttu-id="ad307-149">REG_DWORD</span><span class="sxs-lookup"><span data-stu-id="ad307-149">REG_DWORD</span></span></li> <li><span data-ttu-id="ad307-150">REG_DWORD_LITTLE_ENDIAN</span><span class="sxs-lookup"><span data-stu-id="ad307-150">REG_DWORD_LITTLE_ENDIAN</span></span></li> <li><span data-ttu-id="ad307-151">REG_DWORD_BIG_ENDIAN</span><span class="sxs-lookup"><span data-stu-id="ad307-151">REG_DWORD_BIG_ENDIAN</span></span></li><li><span data-ttu-id="ad307-152">REG_EXPAND_SZ</span><span class="sxs-lookup"><span data-stu-id="ad307-152">REG_EXPAND_SZ</span></span></li> <li><span data-ttu-id="ad307-153">REG_LINK</span><span class="sxs-lookup"><span data-stu-id="ad307-153">REG_LINK</span></span></li> <li><span data-ttu-id="ad307-154">REG_MULTI_SZ</span><span class="sxs-lookup"><span data-stu-id="ad307-154">REG_MULTI_SZ</span></span></li> <li><span data-ttu-id="ad307-155">REG_NONE</span><span class="sxs-lookup"><span data-stu-id="ad307-155">REG_NONE</span></span></li> <li><span data-ttu-id="ad307-156">REG_QWORD</span><span class="sxs-lookup"><span data-stu-id="ad307-156">REG_QWORD</span></span></li> <li><span data-ttu-id="ad307-157">REG_QWORD_LITTLE_ENDIAN</span><span class="sxs-lookup"><span data-stu-id="ad307-157">REG_QWORD_LITTLE_ENDIAN</span></span></li> <li><span data-ttu-id="ad307-158">REG_SZ</span><span class="sxs-lookup"><span data-stu-id="ad307-158">REG_SZ</span></span></li></ul> <span data-ttu-id="ad307-159">可取值为：`unknown`、`binary`、`dword`、`dwordLittleEndian`、`dwordBigEndian`、`expandSz`、`link`、`multiSz`、`none`、`qword`、`qwordlittleEndian`、`sz`。</span><span class="sxs-lookup"><span data-stu-id="ad307-159">Possible values are: `unknown`, `binary`, `dword`, `dwordLittleEndian`, `dwordBigEndian`, `expandSz`, `link`, `multiSz`, `none`, `qword`, `qwordlittleEndian`, `sz`.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="ad307-160">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="ad307-160">JSON representation</span></span>

<span data-ttu-id="ad307-161">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="ad307-161">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.registryKeyState"
}-->

```json
{
  "hive": "@odata.type: microsoft.graph.registryHive",
  "key": "String",
  "oldKey": "String",
  "oldValueData": "String",
  "oldValueName": "String",
  "operation": "@odata.type: microsoft.graph.registryOperation",
  "processId": 1024,
  "valueData": "String",
  "valueName": "String",
  "valueType": "@odata.type: microsoft.graph.registryValueType"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "registryKeyState resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
