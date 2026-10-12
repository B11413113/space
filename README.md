# space

115-1 學期微算機原理及應用課程－程式碼與專案目錄。
fuck

---

## 專案檔案結構與相關連結

<details>
<summary><a href="https://github.com/B11413113/space">space (專案根目錄)</a>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;# GitHub 儲存庫主目錄</summary>
<ul>
  <li>
    <details>
      <summary><a href="https://github.com/B11413113/space/blob/main/Lab2.c">Lab2.c</a>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;# 說明專案內容：EXTI 外部中斷與 NVIC 向量中斷控制器實驗</summary>
      <ul>
        <li>
          <details>
            <summary>Core&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;# 核心應用程式碼目錄</summary>
            <ul>
              <li>
                <details>
                  <summary>Inc&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;# 專案標頭檔目錄</summary>
                  <ul>
                    <li><a href="https://github.com/B11413113/space/blob/main/Lab2.c">main.h&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;# 全域定義與中斷引腳宣告檔</a></li>
                    <li>stm32g4xx_hal_conf.h&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;# HAL 模組啟用配置檔</li>
                    <li>stm32g4xx_it.h&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;# EXTI 外部中斷服務常式標頭檔</li>
                  </ul>
                </details>
              </li>
              <li>
                <details>
                  <summary>Src&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;# 專案 C 語言原始碼目錄</summary>
                  <ul>
                    <li><a href="https://github.com/B11413113/space/blob/main/Lab2.c">main.c (Lab2.c 實作)&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;# 主程式與 HAL_GPIO_EXTI_Callback 中斷觸發回呼邏輯</a></li>
                    <li>stm32g4xx_hal_msp.c&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;# EXTI 引腳與 NVIC 中斷優先級初始化</li>
                    <li>stm32g4xx_it.c&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;# EXTI Line 中斷服務常式 (ISR) 實作</li>
                    <li>system_stm32g4xx.c&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;# 系統時脈與硬體基礎設定</li>
                  </ul>
                </details>
              </li>
              <li>
                <details>
                  <summary>Startup&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;# 開機啟動檔目錄</summary>
                  <ul>
                    <li>startup_stm32g474retx.s&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;# 組合語言啟動與中斷向量表 (Vector Table) 設定檔</li>
                  </ul>
                </details>
              </li>
            </ul>
          </details>
        </li>
        <li>
          <details>
            <summary>Drivers&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;# STM32 官方硬體驅動庫</summary>
            <ul>
              <li>
                <details>
                  <summary>CMSIS&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;# ARM Cortex-M 核心標準抽象層</summary>
                  <ul>
                    <li>Device/ST/STM32G4xx/Include&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;# MCU 暫存器定義標頭檔</li>
                    <li>Include&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;# Cortex-M4 NVIC 中斷控制器標頭檔</li>
                  </ul>
                </details>
              </li>
              <li>
                <details>
                  <summary>STM32G4xx_HAL_Driver&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;# HAL 驅動庫</summary>
                  <ul>
                    <li>Inc&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;# HAL EXTI 與 GPIO 驅動標頭檔</li>
                    <li>Src&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;# HAL EXTI 與 GPIO 驅動原始碼</li>
                  </ul>
                </details>
              </li>
            </ul>
          </details>
        </li>
        <li>
          <details>
            <summary>Debug&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;# 編譯產出目錄</summary>
            <ul>
              <li>Lab2.elf&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;# 可執行與除錯檔</li>
              <li>Lab2.map&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;# 記憶體配置映射檔</li>
            </ul>
          </details>
        </li>
        <li>.cproject&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;# IDE 工具鏈與編譯配置檔</li>
        <li>.project&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;# IDE 專案檔</li>
        <li><a href="https://github.com/B11413113/space/blob/main/Lab2.c">Lab2.ioc (內含設定)&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;# STM32CubeMX 中斷優先級與 EXTI 觸發模式設定檔</a></li>
        <li>STM32G474RETX_FLASH.ld&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;# Linker 連結腳本檔</li>
      </ul>
    </details>
  </li>

  <li>
    <details>
      <summary><a href="https://github.com/B11413113/space/blob/main/lab3.txt">lab3.txt</a>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;# 說明專案內容：Timer 定時器中斷、基頻計數與 PWM 訊號輸出控制實驗</summary>
      <ul>
        <li>
          <details>
            <summary>Core&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;# 核心應用程式碼目錄</summary>
            <ul>
              <li>
                <details>
                  <summary>Inc&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;# 專案標頭檔目錄</summary>
                  <ul>
                    <li><a href="https://github.com/B11413113/space/blob/main/lab3.txt">main.h (lab3 參數)&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;# 主程式全域宣告與 Timer 定時器設定值檔</a></li>
                    <li>stm32g4xx_hal_conf.h&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;# HAL 庫定時器 (TIM) 模組啟用檔</li>
                    <li>stm32g4xx_it.h&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;# 定時器更新中斷標頭檔</li>
                  </ul>
                </details>
              </li>
              <li>
                <details>
                  <summary>Src&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;# 專案 C 語言原始碼目錄</summary>
                  <ul>
                    <li><a href="https://github.com/B11413113/space/blob/main/lab3.txt">main.c (lab3 實作)&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;# HAL_TIM_PeriodElapsedCallback 定時器計數與 PWM 占空比調節</a></li>
                    <li>stm32g4xx_hal_msp.c&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;# TIM 定時器時脈源與 Channel PWM Pin 腳初始化</li>
                    <li>stm32g4xx_it.c&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;# 定時器溢位中斷服務常式實作</li>
                    <li>system_stm32g4xx.c&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;# 系統時脈設定檔</li>
                  </ul>
                </details>
              </li>
            </ul>
          </details>
        </li>
        <li>
          <details>
            <summary>Drivers&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;# STM32 官方硬體驅動庫</summary>
            <ul>
              <li>
                <details>
                  <summary>CMSIS & HAL_Driver&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;# 核心與 HAL 驅動庫</summary>
                  <ul>
                    <li><a href="https://github.com/B11413113/space/blob/main/lab3.txt">lab3.txt 完整參數紀錄檔&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;# 定時器預分頻器 (Prescaler) 與重裝載值 (ARR) 紀錄</a></li>
                  </ul>
                </details>
              </li>
            </ul>
          </details>
        </li>
      </ul>
    </details>
  </li>

  <li>
    <details>
      <summary><a href="https://github.com/B11413113/space/blob/main/work.txt">work.txt</a>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;# 說明專案內容：綜合應用、平時上機作業與專案練習紀錄檔</summary>
      <ul>
        <li>
          <details>
            <summary>Work_Core & Notes&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;# 作業與隨堂練習內容</summary>
            <ul>
              <li><a href="https://github.com/B11413113/space/blob/main/work.txt">work.txt 核心程式與上機筆記&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;# GPIO 基礎輪詢、按鍵控制與整合測試程式碼片段</a></li>
            </ul>
          </details>
        </li>
      </ul>
    </details>
  </li>

  <li><a href="https://github.com/B11413113/space/blob/main/.gitattributes">.gitattributes</a>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;# Git 檔案屬性與行結尾 (Line Endings) 規範設定檔</li>
  <li><a href="https://github.com/B11413113/space/blob/main/.gitignore">.gitignore</a>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;# Git 忽略版本控制設定檔（包含 *.o, *.elf 等暫存檔過濾）</li>
  <li><a href="https://github.com/B11413113/space/blob/main/README.md">README.md</a>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;# 本儲存庫主說明文件與專案結構導覽</li>
</ul>
</details>